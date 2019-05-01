<template>
<div>
    <h1>{{component.citation}}</h1>
    <h2>{{component.authors}}</h2>
</div>
    
</template>

<script>
export default {
    name : 'Citation',
    props : ['component']
}
</script>

<style>

</style>
