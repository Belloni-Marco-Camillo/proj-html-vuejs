<template>
  <div id="app">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <HeaderSite/>

    <MainSite/>

    <FooterSite/>
  </div>
</template>

<script>
/* import HelloWorld from './components/HelloWorld.vue' */
import HeaderSite from './components/HeaderComponents/HeaderSite.vue'
import MainSite from './components/MainComponents/MainSite.vue'
import FooterSite from './components/FooterComponents/FooterSite.vue'

export default {
  name: 'App',
  components: {
    /* HelloWorld, */
    HeaderSite,
    MainSite,
    FooterSite
  },
}
</script>

<style lang="scss">
#app {
  font-family: 'Roboto Slab', serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
 
}
</style>
