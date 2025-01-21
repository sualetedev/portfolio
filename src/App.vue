<template>
  <CabeceraInicio />
  <PhotoLinks :buttons="[
        { text: 'GitHub', link: 'https://github.com/sualetedev', variant: 'dark', icon: 'fab fa-github' },
        { text: 'LinkedIn', link: 'https://www.linkedin.com/in/alejandro-izquierdo-garcia-8333a9114/', variant: 'primary', icon: 'fab fa-linkedin' }
      ]"
    />
</template>

<script>
import CabeceraInicio from './components/CabeceraInicio.vue'
import PhotoLinks from './components/PhotoLinks.vue';

export default {
  name: 'App',
  components: {
    CabeceraInicio, PhotoLinks,
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
