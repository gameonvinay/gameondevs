<template>
  <div>
    <ul>
      <li v-for="color of colors" :key="color"
        ><component
          :is="`icon-${color}`"
          @click="$colorMode.preference = color"
          :class="getClasses(color)"
        />
      </li>
    </ul>
    <!-- <p>
      <ColorScheme placeholder="..." tag="span">
        <b>{{ $colorMode.preference }}</b>
        <span v-if="$colorMode.preference === 'system'"
          >(<i>{{ $colorMode.value }}</i> mode detected)</span
        >
      </ColorScheme>
    </p> -->
  </div>
</template>
<script>
import IconLight from '@/assets/icons/light.svg?inline'
import IconDark from '@/assets/icons/dark.svg?inline'

export default {
  components: {
    IconLight,
    IconDark,
  },
  data() {
    return {
      colors: ['system', 'light', 'dark'],
    }
  },
  methods: {
    getClasses(color) {
      if (this.$colorMode.unknown) {
        return {}
      }
      return {
        preferred: color === this.$colorMode.preference,
        selected: color === this.$colorMode.value,
      }
    },
  },
}
</script>
<style scoped></style>
