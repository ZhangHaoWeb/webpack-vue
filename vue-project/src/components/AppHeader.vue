<template>
  <div class="app-header">
    {{headerMessage}}
  </div>
</template>

<script>
  export default {
    name:"AppHeader",
    data () {
      return{
        headerMessage:'this is common header'
      }
    }
  }
</script>


<style scoped>
  .app-header{
    background: gray;
    height: 60px;
    line-height: 60px;
  }
</style>
