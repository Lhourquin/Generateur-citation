<template class="citation">
<div>
    
    <div class="container-citation" 

    v-for="(component) in componentDisplay" 
    :key="component.id">
    <h1>{{component.id.citation}}</h1>
    <h2>{{component.id.authors}}</h2>
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
      ],
      index : null,
      componentDisplay : [],
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
.citation{
grid-area : citation;

}
.container-citation{

text-align: center;
margin : 15vw;
}
h2{
margin-left: 30vw;
margin-top : 10vh;
}
button{
text-align: center;
}

</style>
