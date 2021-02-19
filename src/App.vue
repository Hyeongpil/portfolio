<template>
  <div id="app" class="html-container">
    <sb-header />
    <div class="container content-container">
      <first-section class="first-container" />
      <about-section />
    </div>
  </div>
</template>

<script>
import SbHeader from "./components/SbHeader.vue"
import FirstSection from "./components/FirstSection.vue"
import AboutSection from "./components/AboutSection.vue"

export default {
  name: "App",
  components: {
    SbHeader,
    FirstSection,
    AboutSection
  }
}
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Gothic+A1:wght@400;500;600;700;800;900&display=swap");

#app {
  font-family: "Gothic A1", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

html {
  background: #121212;
  background-repeat: no-repeat;
  background-position: top center;
  background-size: cover;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  min-width: 100%;
  min-height: 100%;
}

.content-container {
  display: flex;
  flex-direction: column;
  margin-top: 200px;
}

.first-container {
  height: 800px;
}

.html-container {
  margin-bottom: 150px;
}
</style>
