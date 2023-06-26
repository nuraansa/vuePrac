<template>
  <Nav/>
  <router-view/>
  <Userdata/>
  <Footer/>
</template>

<script>
import Footer from '@/components/Footer';
import Nav from '@/components/Nav.vue';
import Userdata from '@/components/Data.vue';
  export default {
    components: {
      Footer,Nav,Userdata
    }
  }
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: black;
}
</style>
