<template>
  <div id="app">
    <Header />
    <Jumbo />
    <PageNav />
  </div>
</template>



<script>

import Header from './components/Header.vue'
import Jumbo from './components/Jumbo.vue'
import PageNav from './components/PageNav.vue'



export default {
  name: 'App',
  components: {
    Header,
    Jumbo,
    PageNav
  }
}
</script>

<style lang="scss">
@import './style/variables.scss';



#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50; 
}
</style>
