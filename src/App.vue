<template>
  <div id="app">
    
    <HeaderSite/>

    <MainSite/>

    <FooterSite/>
    
  </div>
</template>

<script>

import HeaderSite from './components/HeaderComponents/HeaderSite.vue'
import MainSite from './components/MainComponents/MainSite.vue'
import FooterSite from './components/FooterComponents/FooterSite.vue'

export default {
  name: 'App',
  components: {
    HeaderSite,
    MainSite,
    FooterSite
  },
}
</script>

<style lang="scss">
@import "@/assets/scss/style.scss"

</style>
