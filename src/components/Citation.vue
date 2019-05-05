<template>
<div>
    <div 
    v-for="(component) in componentDisplay" 
    :key="component.id">
    <h1>{{component.id}}</h1>
    </div>
    <button
    v-on:click="eventRandom"
    >Random</button>
</div>
    
</template>

<script>
export default {
    name : 'Citation',
    data () {
    return {
      componentNames : [
        'On se prend souvent pour quelqu\'un, alors qu\'au fond, on est plusieurs. Raymond Devos',

        'Exige beaucoup de toi-même et attends peu des autres. Ainsi beaucoup d\'ennuis te seront épargnés. Confucius',

        'La vie, c\'est comme une bicyclette, il faut avancer pour ne pas perdre l\'équilibre. Albert Einstein',

        'Qu\'est ce que l\'homme, si le bien suprême, l\'aubaine de sa vie est uniquement de dormir et de manger ? ... Une bête, rien de plus. William Shakespeare',

        'Si quelqu\'un t\'a offensé, ne cherche pas à te venger. Assieds-toi au bord de la rivière et bientôt tu verras passer son cadavre. Lao Tseu'
      ],
      index : null,
      componentDisplay : []
    }
},
    methods : {
        getRandom : function () {
            this.index = this.componentNames[Math.floor(Math.random() * this.componentNames.length)]
        },
        pushRandom : function () {
            this.componentDisplay.push({
                id :this.index
            })
        },
        popRandom : function () {
            if(this.componentDisplay.length > 1)
            this.componentDisplay.shift()
        },
        eventRandom : function () {
            this.getRandom()
            this.pushRandom()
            this.popRandom()
        }
    }
}

</script>

<style>

</style>
