<template>
  <div id="app">
    <Citation v-for="component in componentNames" :key="component" :component="component"/>
  </div>
</template>

<script>
import Citation from './components/Citation.vue'


export default {
  name: 'app',
  components : {
    Citation
  },
  data () {
    return {
      componentNames : [
        {citation : 'On se prend souvent pour quelqu\'un, alors qu\'au fond, on est plusieurs.',
        authors : 'Raymond Devos'},

        {citation : 'Exige beaucoup de toi-même et attends peu des autres. Ainsi beaucoup d\'ennuis te seront épargnés.',
        authors : 'Confucius'},

        {citation : 'La vie, c\'est comme une bicyclette, il faut avancer pour ne pas perdre l\'équilibre.',
        authors : 'Albert Einstein'},

        {citation : 'Qu\'est ce que l\'homme, si le bien suprême, l\'aubaine de sa vie est uniquement de dormir et de manger ? ... Une bête, rien de plus.',
        authors : 'William Shakespeare'},

        {citation : 'Si quelqu\'un t\'a offensé, ne cherche pas à te venger. Assieds-toi au bord de la rivière et bientôt tu verras passer son cadavre.',
        authors : 'Lao Tseu'}
      ]
    }
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
