<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <h3>
      <router-link to="/index">Go to index page.</router-link>
    </h3>
    <button v-on:click="say">点击触发事件{{events}}</button>   


  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      events:true
    }
  },
  methods:{
    say() {
      console.log(this.events)
      if (this.events) {
        this.events = 'this is a click event.';
        console.log(this.events);
      }else{
        console.log('events error...');
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
