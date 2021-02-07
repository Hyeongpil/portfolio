<template>
  <div id="app">
    <sb-header/>
    <first-section/>
    <about-section/>
    
  </div>
</template>

<script>
import SbHeader from './components/SbHeader.vue'
import FirstSection from './components/FirstSection.vue'
import AboutSection from './components/AboutSection.vue'



export default {
  name: 'App',
  components: {
    SbHeader,
    FirstSection,
    AboutSection,
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
