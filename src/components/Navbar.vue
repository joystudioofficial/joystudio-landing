<template>
  <div>
    <nav class="js-navigation">
      <div class="container cf">
        <div class="js-navigation-brand">
          <a href="http://" class="js-navigation-logo">Joy <span style="color: #1DD1A1;">Studio.</span></a>
        </div>

        <button class="btn btn-open-side-bar" id="btnOpenSideMenu" @click="showSidebar">
          <img src="@/assets/images/menu.svg" class="menu-bar" alt="" srcset="">
        </button>

        <div class="js-navigation-menu">
          <ul class="js-nav-menu">
            <li class="js-nav-item"><a href="#about-js-section" class="js-nav-link" v-smooth-scroll>About</a></li>
            <li class="js-nav-item"><a href="#js-services-section" class="js-nav-link" v-smooth-scroll>Services</a></li>
            <li class="js-nav-item"><a href="#js-portfolio-section" class="js-nav-link" v-smooth-scroll>Portfolio</a></li>
          </ul>
        </div>
      </div>
    </nav>

    <section class="js-side-bar-overlay" id="sidebar" :class="{'active' : sidebarOverlay}">
      <aside class="js-side-bar">
        <div class="container">
          <div class="js-side-header">
            <div class="js-side-menu-brand">
              <a href="#" class="js-side-menu-logo">Joy <span style="color: var(--primary-color);">Studio.</span></a>
            </div>
            <button class="btn btn-close-side-bar" id="btnCloseSideMenu" @click="closeSidebar">
              <span>&times;</span>
            </button>
          </div>

          <div class="js-side-section-menu">
            <ul class="js-side-menu">
              <li class="js-side-item"><a href="#about-js-section" class="js-side-link" v-smooth-scroll>About</a></li>
              <li class="js-side-item"><a href="#js-services-section" class="js-side-link" v-smooth-scroll>Services</a></li>
              <li class="js-side-item"><a href="#js-portfolio-section" class="js-side-link" v-smooth-scroll>Portfolio</a></li>
            </ul>
          </div>
        </div>
      </aside>
    </section>
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      sidebarOverlay: false
    }
  },

  methods: {
    showSidebar() {
      this.sidebarOverlay = !this.sidebarOverlay 
    },

    closeSidebar() {
      this.sidebarOverlay = !this.sidebarOverlay
    }
  }
}
</script>
