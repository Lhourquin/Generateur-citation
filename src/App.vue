<template>
  <div id="app">
    <Citation />
  </div>
</template>

<script>
import Citation from './components/Citation.vue'


export default {
  name: 'app',
  components : {
    Citation
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
