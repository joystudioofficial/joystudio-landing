<template>
  <div class="home">
    <!-- Landing Area -->
    <LandingArea></LandingArea>

    <!-- Home Content -->
    <HomeContent></HomeContent>
  </div>
</template>

<script>

import LandingArea from '@/components/LandingArea.vue'

import HomeContent from '@/components/HomeContent.vue'

export default {
  name: 'home',
  components: {
    LandingArea,
    HomeContent
  }
}
</script>