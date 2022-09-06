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
  
  .container{
    max-width: 1200px;
    margin: 0 auto;
    
    
  }
  body{
    margin: 0;
  }
  
  



</style>
