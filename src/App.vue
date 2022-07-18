<template>
  <div id="app">
    <Header/>
    <MainBanner/>
    <MainProducts/>
    <FooterLinks/>
    <FooterInfo/>

  </div>
</template>

<script>
import Header from './components/Header.vue'
import MainBanner from './components/MainBanner.vue'
import MainProducts from './components/MainProducts.vue'
import FooterInfo from './components/FooterInfo.vue'
import FooterLinks from './components/FooterLinks.vue'


export default {
  name: 'App',
  components: {
    Header,
    MainBanner,
    MainProducts,
    FooterLinks,
    FooterInfo,

  }
}
</script>

<style lang="scss">
#app {
@import "~bootstrap/scss/bootstrap.scss";
// Font
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');

}

body{
  font-family: 'Open Sans', sans-serif;
  overflow-x: hidden;
  margin: 0;
  padding: 0;
}

</style>
