<template>
  <div class="home">
    <Navbar></Navbar>

    <LandingArea></LandingArea>
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from '@/components/Navbar.vue'
import LandingArea from '@/components/LandingArea.vue'

import './../../node_modules/milligram/dist/milligram.min.css'

export default {
  name: 'home',
  components: {
    Navbar,
    LandingArea
  }
}
</script>