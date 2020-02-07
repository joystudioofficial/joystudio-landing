<template>
  <div>
    <nav class="js-navigation">
      <div class="container cf">
        <div class="js-navigation-brand">
          <a href="http://" class="js-navigation-logo">Joy <span style="color: #1DD1A1;">Studio.</span></a>
        </div>

        <button class="btn btn-open-side-bar" id="btnOpenSideMenu">
          <img src="@/assets/images/menu.svg" class="menu-bar" alt="" srcset="">
        </button>

        <div class="js-navigation-menu">
          <ul class="js-nav-menu">
            <li class="js-nav-item"><a href="http://" class="js-nav-link">About</a></li>
            <li class="js-nav-item"><a href="http://" class="js-nav-link">Services</a></li>
            <li class="js-nav-item"><a href="http://" class="js-nav-link">Portfolio</a></li>
            <li class="js-nav-item"><a href="http://" class="js-nav-link">Contact</a></li>
          </ul>
        </div>
      </div>
    </nav>

    <section class="js-side-bar-overlay" id="sidebar">
      <aside class="js-side-bar">
        <div class="container">
          <div class="js-side-header">
            <div class="js-side-menu-brand">
              <a href="http://" class="js-side-menu-logo">Joy <span>Studio.</span></a>
            </div>
            <button class="btn btn-close-side-bar" id="btnCloseSideMenu">
              <span>&times;</span>
            </button>
          </div>

          <div class="js-side-section-menu">
            <ul class="js-side-menu">
              <li class="js-side-item"><a href="http://" class="js-side-link">About</a></li>
              <li class="js-side-item"><a href="http://" class="js-side-link">Services</a></li>
              <li class="js-side-item"><a href="http://" class="js-side-link">Portfolio</a></li>
              <li class="js-side-item"><a href="http://" class="js-side-link">Contact</a></li>
            </ul>
          </div>
        </div>
      </aside>
    </section>
  </div>
</template>

<script>
import '@/assets/front-assets/js/myscript.js'

export default {
  
}
</script>