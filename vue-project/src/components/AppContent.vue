<template>
  <div class="app-content">
    {{msg}}
    <div>
      <router-link to="/">back to root</router-link>
    </div>
    <app-menu></app-menu>
  </div>
</template>

<script>
  import AppMenu from './AppMenu.vue'
  export default {
    name:'AppContent',
    data () {
      return {
        msg:'this is content'
      }
    },
    components:{
      'app-menu':AppMenu
    }
  }
</script>

<style lang="css">
    .app-content{
      position: fixed;
      top: 60px;
      bottom: 60px;
      left: 0;
      right: 0;
      background: green;
    }

</style>
