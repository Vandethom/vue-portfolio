<template>
  <div>
    <Banner />
    <Navbar />
  </div>
</template>

<script>
import Banner from './components/Banner'
import Navbar from './components/Navbar'

export default {
  name: 'App',
  components: {
    Banner,
    Navbar
  }
}
</script>

<style>
body {
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  margin: 0;
  scroll-behavior: smooth;
}
</style>
