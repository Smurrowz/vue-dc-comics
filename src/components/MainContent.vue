<template >
  <main>
    <MainCard/>
  </main>
</template>
<script>
import MainCard from './MainCard.vue';
  
  export default{
    name: "MainContent",
    data() {
        return {};
    },
    components: { MainCard }
}
</script>
<style scoped lang="scss">
  main{
    background-color: rgba(0, 0, 0, 0.899);
    padding: 50px 0;
    color: white;
    font-size: 2rem;
  }
</style>