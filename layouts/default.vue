<template>
  <div>
    <header class="main-header">
      <section class="section-theme">
        <div class="notification">#BlackLivesMatter</div>
        <ColorModePicker class="color-mode-picker" />
      </section>
      <nav id="mynav" class="nav-container-desktop">
        <h2 class="logo">
          GAME ON DEVS
        </h2>
        <div>
          <ul class="nav-items">
            <li class="nav-item">
              <a class="animation-hover" href="#">Projects</a>
            </li>
            <li class="nav-item">
              <a class="animation-hover" href="#">Technology</a>
            </li>
            <li class="nav-item">
              <a class="animation-hover" href="#">About Us</a>
            </li>
          </ul>
        </div>
        <div class="nav-btn">
          <button>LOGIN</button>
          <button class="btn-signup">SIGN UP</button>
        </div>
      </nav>
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
    <footer class="footer-section">
      <section class="footer-section-social-media">
        <h2>Features</h2>
        <a href="#">Twitter</a>
        <a href="#">Facebook</a>
        <a href="#">Instagram</a>
        <a href="#">YouTube</a>
        <a href="#">Discord</a>
      </section>
      <section class="footer-section-website-type">
        <h2>Company</h2>
        <a href="#">Customer Reviews</a>
        <a href="#">Jobs</a>
        <a href="#">About Us</a>
        <a href="#">Contact Us</a>
        <a href="#">Blog</a>
      </section>
      <section class="footer-section-tech-stack">
        <h2>Support</h2>
        <a href="#">Help Centre</a>
        <a href="#">Terms of Service</a>
        <a href="#">Privacy</a>
        <a href="#">Security</a>
        <a href="#">Resources</a>
      </section>
      <section class="footer-section-misc-links">
        <h2>Follow</h2>
        <a href="#">Twitter</a>
        <a href="#">Facebook</a>
        <a href="#">Instagram</a>
        <a href="#">Discord</a>
        <a href="#">YouTube</a>
      </section>
      <section class="footer-section-copyright">
        <div>
          Copyright &copy; 2020 Game On Developers. &nbsp;
        </div>
        <div>
          All rights reserved.
        </div>
      </section>
    </footer>
  </div>
</template>
<script>
import ColorModePicker from '@/components/ColorModePicker'

export default {
  components: { ColorModePicker },
}
</script>
<style></style>
