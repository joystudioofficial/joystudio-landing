<template>
  <div id="app">
    <!-- Navbar -->
    <Navbar></Navbar>


    <!-- footer -->

    <router-view/>
  </div>
</template>

<script>

import Navbar from "@/components/Navbar.vue"

export default {
  name: "app",
  components: {
    Navbar
  }
}
</script>

<style>
@import './assets/front-assets/css/style.css';
@import './../node_modules/milligram/dist/milligram.min.css';

#app {
  text-align: center;
}
</style>
