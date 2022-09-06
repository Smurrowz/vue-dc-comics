<template>
  <div id="app">
    <MainHeader></MainHeader>
    <HeroJumbodron/>
    <MainContent></MainContent>
    <MainFooter></MainFooter>
    
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue';
import MainContent from './components/MainContent.vue';
import MainFooter from './components/MainFooter.vue';
import HeroJumbodron from './components/HeroJumbodron.vue';


export default {
    name: "App",
    components: { MainHeader, MainContent, MainFooter, HeroJumbodron }
}
</script>

<style lang="scss">
  @import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,300;0,400;0,500;0,700;1,300;1,400;1,500;1,700&display=swap');
  
  
  .container{
    max-width: 1200px;
    margin: 0 auto;
    
    
    
  }
  body{
    margin: 0;
    font-family: 'Roboto', sans-serif;
  }
 
  



</style>
