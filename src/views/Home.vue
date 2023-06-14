<template>
  <Navbar/>
  <Carousels/>
  <AboutMe/>
  <Projects/>
</template>

<script>
import Navbar from '../components/shared/Navbar.vue'
import Carousels from '../components/Home/Carousels.vue'
import AboutMe from '../components/Home/AboutMe.vue'
import Projects from '../components/Home/Projects.vue'
export default {
  components:{ Navbar, Carousels, AboutMe, Projects}
}
</script>

<style>

</style>