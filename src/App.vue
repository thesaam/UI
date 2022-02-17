<script>
  import Navbar from './components/Navbar.vue'
  import Button from './components/Button.vue'
  import Header from './components/Header.vue'
  import Overview from './components/Overview.vue'

  export default {

    components: {
      Navbar,
      Button,
      Header,
      Overview
    }
  }

</script>

<template>
  <header class="container-fluid">
    <Navbar />
    <Header/> 
  </header>
  <main>
    <Overview />
    
  </main>
</template>

<style>
@import "./assets/base.css";

/* #app {
  max-width: 1280px;
  margin: 0 auto;

  font-weight: normal;
} */


</style>
