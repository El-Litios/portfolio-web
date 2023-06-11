<template>
  <Navbar/>
  <Carousels/>
  <AboutMe/>
</template>

<script>
import Navbar from '../components/shared/Navbar.vue'
import Carousels from '../components/Home/Carousels.vue'
import AboutMe from '../components/Home/AboutMe.vue'
export default {
  components:{ Navbar, Carousels, AboutMe}
}
</script>

<style>

</style>