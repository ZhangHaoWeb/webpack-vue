<template>
  <div class="app-footer">
    {{footerMessage}}
  </div>
</template>

<script>
  export default {
    name:'AppFooter',
    data () {
      return {
        footerMessage:'this is common footer'
      }
    }
  }
</script>

<style scoped>
  .app-footer{
    position: fixed;
    left: 0;
    right: 0;
    bottom: 0;
    background: gray;
    height: 60px;
    line-height: 60px;
  }
</style>
