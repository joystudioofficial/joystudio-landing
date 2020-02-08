<template>
  <div class="home">
    <!-- Landing Area -->
    <LandingArea></LandingArea>

    <!-- Home Content -->
    <HomeContent></HomeContent>

    <!-- Footer -->
    <Footer></Footer>
  </div>
</template>

<script>

import LandingArea from '@/components/LandingArea.vue'

import HomeContent from '@/components/HomeContent.vue'

import Footer from '@/components/Footer.vue'

export default {
  name: 'home',
  components: {
    LandingArea,
    HomeContent,
    Footer
  }
}
</script>