<template>
  <div>
    <Banner />
    <Navbar />
    <About />
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


export default {
  name: 'App',
  components: {
    Banner,
    Navbar,
    About
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
