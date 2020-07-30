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
<style scoped>
.feather {
  cursor: pointer;
  padding: 4px;
  background-color: var(--color-background);
  outline: 1px solid var(--color-background);
  margin: 0;
  border-radius: 5px;
  transition: all 0.1s ease;
}
.feather:hover {
  border-color: var(--color-text-nav);
}
.feather.preferred {
  border-color: var(--color-text-nav);
}
.feather.selected {
  color: var(--color-white);
  border-color: var(--color-text-nav);
  background-color: var(--color-primary-theme);
}
ul {
  list-style-type: none;
  display: flex;
}
</style>
