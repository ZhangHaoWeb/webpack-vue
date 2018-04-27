<template>
  <div class="app-menu">
    <ul>
      <li v-for="l in menu">{{l.list}}</li>
    </ul>
  </div>
</template>

<script>
  export default {
    name:'AppMenu',
    data(){
      return {
        menu:[{
          list:'vue'
        },{
          list:'angular'
        },{
          list:'react'
        }]
      }
    }
  }
</script>

<style>
  .app-menu{
    position: fixed;
    left: 0;
    width: 120px;
    top:60px;
    bottom: 60px;
    background: gold;
  }
</style>
