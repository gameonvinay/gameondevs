<template>
  <div>
    <header class="main-header">
      <section class="section-theme">
        <div class="notification">#BlackLivesMatter</div>
        <ColorModePicker class="color-mode-picker" />
      </section>
      <nav id="mynav" class="nav-container">
        <h2 class="logo">
          GAME ON DEVS
        </h2>
        <svg
          class="svg-menu"
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 24 24"
        >
          <path d="M0 0h24v24H0V0z" fill="none" />
          <path
            d="M4 18h16c.55 0 1-.45 1-1s-.45-1-1-1H4c-.55 0-1 .45-1 1s.45 1 1 1zm0-5h16c.55 0 1-.45 1-1s-.45-1-1-1H4c-.55 0-1 .45-1 1s.45 1 1 1zM3 7c0 .55.45 1 1 1h16c.55 0 1-.45 1-1s-.45-1-1-1H4c-.55 0-1 .45-1 1z"
          />
        </svg>
      </nav>
    </header>
    <nuxt />
  </div>
</template>
<script>
import ColorModePicker from '@/components/ColorModePicker'

export default {
  components: { ColorModePicker },
}
</script>
<style></style>
