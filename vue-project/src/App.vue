<template>
  <div id="app">
    <app-header></app-header>

      <router-view/>

    <app-footer></app-footer>
  </div>
</template>

<script>
  import AppHeader from './components/AppHeader.vue'
  import AppContent from './components/AppContent.vue'
  import AppFooter from './components/AppFooter.vue'

  export default {
    components:{
      'app-header':AppHeader,
      'app-footer':AppFooter,
      'app-content':AppContent
    }
  }
</script>

<style>
  *{
    margin: 0;
    padding: 0;
  }
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }
</style>
