<template>
<!--  <img alt="Vue logo" src="./assets/backimg.png">-->
    <home msg="Welcome to Your Vue.js App"/>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import home from './components/home'
export default {
  name: 'App',
  components: {
    home
  },
  data() {
    return {

    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
}
.home{
  min-height: max-content;
}
</style>
