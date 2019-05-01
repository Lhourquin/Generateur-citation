<template>
  <div id="app">
    <CitationHamlet/>
    <CitationConfucius/>
    <citation-jean-paul/>
    <citation-albert/>
    <citation-raymond/>
  </div>
</template>

<script>
import CitationHamlet from './components/CitationHamlet.vue'
import CitationConfucius from './components/CitationConfucius.vue'
import CitationJeanPaul from './components/CitationJeanPaul.vue'
import CitationAlbert from './components/CitationAlbert.vue'
import CitationRaymond from './components/CitationRaymond.vue'


export default {
  name: 'app',
  components: {
    CitationHamlet,
    CitationConfucius,
    CitationJeanPaul,
    CitationAlbert,
    CitationRaymond
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
