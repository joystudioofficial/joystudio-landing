<template>
  <div id="app">
    <!-- Navbar -->
    <Navbar></Navbar>
    <router-view/>
  </div>
</template>

<script>

import Navbar from "@/components/Navbar.vue"

import './../node_modules/milligram/dist/milligram.min.css'

export default {
  name: "app",
  components: {
    Navbar
  }
}
</script>

<style>
@import './assets/front-assets/css/style.css';
#app {
  text-align: center;
}
</style>
