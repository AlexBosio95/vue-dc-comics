<template>
  <div id="app">
    <MainHeader/>
    <MainBanner/>
    <MainProducts/>
    <MainFooterLinks/>
    <MainFooterInfo/>

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
    MainFooterLinks,
    MainFooterInfo,

  }
}
</script>

<style lang="scss">
#app {
@import "~bootstrap/scss/bootstrap.scss";
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');

}

body{
  font-family: 'Open Sans', sans-serif;
  overflow-x: hidden;
  margin: 0;
  padding: 0;
}

</style>
