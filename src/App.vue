<template>
  <div id="app">
   
    <Header1 />
    <MainTop />
   
    
  </div>

</template>

<script>
import MainTop from './components/MainTop.vue'
import Header1 from './components/Header1.vue'

export default {
  name: 'App',
  components: {
    MainTop,
    Header1
}
}
</script>

<style lang="scss">
  @import "~bootstrap/scss/bootstrap.scss";
  @import "./styles/style.scss";
</style>
