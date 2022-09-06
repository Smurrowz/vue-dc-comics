<template>
  <div class="hero">
    <div class="container">
      <button>CURRENT SERIES</button>
    </div>
  </div>
</template>
<script>
  export default {
    name: 'HeroJumbodron'
  }
</script>
<style scoped lang="scss">
  @import '../styles/variables';
  .hero{
    height: 500px;
    background-image:url(../assets/img/jumbotron.jpg) ;
    background-size: cover;
    position: relative;

  }
  button{
    padding: 5px 10px;
    background-color: $my-blue;
    color: white;
    font-size: 1.60rem;
    font-weight: bold;
    transform: translateY(50%);
    border: none;
    position: absolute;
    bottom: 0;
    
  }
</style>