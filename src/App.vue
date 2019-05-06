<template>
  <div id="app" class="container">
    
    <Header/>
    <Citation/>
    <Footer/>
    <SideBar/>
  </div>
</template>

<script>
import Citation from './components/Citation.vue'
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import SideBar from './components/SideBar.vue'

export default {
  name: 'app',
  components : {
    Citation,
    Header,
    SideBar,
    Footer
  }
  
  }
  

</script>

<style>
.container{
display : grid;
text-align: center;
  grid-template-areas: "header citation"
                      
                       "sidebar citation"
                       
                       "sidebar footer";
}
</style>
