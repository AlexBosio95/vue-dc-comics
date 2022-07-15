<template>
  <div id="app">
    <MainHeader/>
    <MainBanner/>
    <MainProducts/>
    <MainFooterInfo/>
    <MainFooterLinks/>
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue'
import MainBanner from './components/MainBanner.vue'
import MainProducts from './components/MainProducts.vue'
import MainFooterInfo from './components/MainFooterInfo.vue'
import MainFooterLinks from './components/MainFooterLinks.vue'


export default {
  name: 'App',
  components: {
    MainHeader,
    MainBanner,
    MainProducts,
    MainFooterInfo,
    MainFooterLinks
  }
}
</script>

<style lang="scss">
#app {
@import "~bootstrap/scss/bootstrap.scss";

}
</style>
