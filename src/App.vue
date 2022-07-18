<template>
  <div id="app">
   
    <Header1 />
    <MainTop />
    <MainBottom />
    <FooterTop />   
    <FooterBottom />  
    
  </div>

</template>

<script>
import Header1 from './components/Header1.vue'
import MainTop from './components/MainTop.vue'
import MainBottom from './components/MainBottom.vue'
import FooterTop from './components/FooterTop.vue'
import FooterBottom from './components/FooterBottom.vue'

export default {
  name: 'App',
  components: {
    Header1,
    MainTop,
    MainBottom,
    FooterTop,
    FooterBottom
}
}
</script>

<style lang="scss">
  @import "~bootstrap/scss/bootstrap.scss";
  @import "./styles/style.scss";
</style>
