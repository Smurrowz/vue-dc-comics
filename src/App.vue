<template>
  <div id="app">
    <MainHeader></MainHeader>
    <MainContent></MainContent>
    <MainFooter></MainFooter>
    
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue';
import MainContent from './components/MainContent.vue';
import MainFooter from './components/MainFooter.vue';


export default {
    name: "App",
    components: { MainHeader, MainContent, MainFooter }
}
</script>

<style lang="scss">
  
  .container{
    max-width: 1200px;
    margin: 0 auto;
    
    
  }
  
  



</style>
