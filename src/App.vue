<template>
  <div>
    <Banner />
    <Navbar />
    <About />
    <Projects />
  </div>
</template>

<script>
import { defineAsyncComponent } from 'vue'

// importing asyncComponents instead of regular ones not to slow the application in case of low loading
const Banner = defineAsyncComponent(() => 
  import("./components/Banner"))
const Navbar = defineAsyncComponent(() => 
  import("./components/Navbar"))
const About = defineAsyncComponent(() => 
  import("./components/About"))
const Projects = defineAsyncComponent(() => 
  import("./components/Projects"))


export default {
  name: 'App',
  components: {
    Banner,
    Navbar,
    About,
    Projects
  }
}
</script>

<style>
body {
  font-family: 'Calibri, Gill Sans', 'Gill Sans MT', 'Trebuchet MS', sans-serif;
  margin: 0;
  scroll-behavior: smooth;
}
</style>
