<template>
  <the-header
      :link="link"
      :count="count"
      @inc_value="count++"
  ></the-header>
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Header from './components/TheHeader.vue'


export default {
  name: 'App',
  components: {
    HelloWorld,
    'the-header': Header
  },
  data() {
    return {
      link: 'Some link',
      count: 0
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
  margin-top: 60px;
}
</style>
