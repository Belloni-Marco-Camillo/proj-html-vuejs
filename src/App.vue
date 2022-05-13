<template>
  <div id="app" class="container">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <HeaderSite/>

    <MainSite/>
  </div>
</template>

<script>
/* import HelloWorld from './components/HelloWorld.vue' */
import HeaderSite from './components/HeaderComponents/HeaderSite.vue'
import MainSite from './components/MainComponents/MainSite.vue'

export default {
  name: 'App',
  components: {
    /* HelloWorld, */
    HeaderSite,
    MainSite
}
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
