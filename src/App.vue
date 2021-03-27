<template>
  <div>
    <Banner />
    <Navbar />
    <About />
    <Projects />
    <Contact />
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
const Contact = defineAsyncComponent(() => 
  import("./components/Contact"))


export default {
  name: 'App',
  components: {
    Banner,
    Navbar,
    About,
    Projects,
    Contact,
  }
}
</script>

<style>
  html {    
        scroll-behavior: smooth;
  }

  body {
    font-family: 'Calibri, Gill Sans', 'Gill Sans MT', 'Trebuchet MS', sans-serif;
    margin: 0;
  }

  @media all and (max-width: 1024px) {
    html {
      width: 100%;
      margin-right: 0;
    }
  }

</style>
