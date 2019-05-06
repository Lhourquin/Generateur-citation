<template class="sidebar">
<div class="container-sidebar">
    <a href="">Twitter</a>
    <a href="">Github</a>
</div>
    
</template>

<script>
export default {
    name : 'SideBar'
}
</script>

<style>
.sidebar{
grid-area: sidebar;
}
.container-sidebar{
display : flex;
flex-direction: column;
}

</style>
