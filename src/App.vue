<template>
  <div id="app">
    <CitationHamlet/>
  </div>
</template>

<script>
import CitationHamlet from './components/CitationHamlet.vue'

export default {
  name: 'app',
  components: {
    CitationHamlet
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
