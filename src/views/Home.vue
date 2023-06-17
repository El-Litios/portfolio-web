<template>
  <Navbar/>
  <Carousels/>
  <AboutMe/>
  <Projects/>
  <Experience/>
  <Footer />
</template>

<script>
import Navbar from '../components/shared/Navbar.vue'
import Footer from '../components/shared/Footer.vue'
import Carousels from '../components/Home/Carousels.vue'
import AboutMe from '../components/Home/AboutMe.vue'
import Projects from '../components/Home/Projects.vue'
import Experience from '../components/Home/Experience.vue'
export default {
  components:{ Navbar, Carousels, AboutMe, Projects, Experience, Footer}
}
</script>

<style>

</style>