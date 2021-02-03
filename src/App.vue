<template>
  <div id="app">
    <sb-header-vue />
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import SbHeaderVue from './components/SbHeader.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    SbHeaderVue
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

html { 
    background: #121212;
    background-repeat:no-repeat;
    background-position:top center;
    background-size: cover;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    min-width: 100%;
    min-height: 100%;
    
}
</style>
