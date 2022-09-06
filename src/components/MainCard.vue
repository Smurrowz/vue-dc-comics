<template>
  <div class="container card-container">
    <div v-for="(card, index) in cards" :key="index" class="card">
      <div>
        <img  class="card-img" :src="card.thumb" :alt="card.series">
      </div>
      <div class="card-bottom">
        <p>{{card.series}}</p>
        <p>{{card.price}}</p>
      </div>
    </div>
    <button>LOAD MORE</button>
  </div>
</template>
<script>
import cards from '../dc-comics'
export default {
  name: 'MainCard',
  data() {
    return {
      cards: cards,

    }
  }
}

</script>
<style scoped lang="scss">
  @import '../styles/variables.scss';
.card-container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr;
  gap: 20px;
  position: relative;
  
  & button{
    padding: 8px 25px;
    color: white;
    background-color: $my-blue;
    position: absolute;
    left: 50%;
    bottom: -40px;
    transform: translateX(-50%);
  }
  & .card {
    margin-bottom: 20px;
    & .card-img {
      object-fit: cover;
      aspect-ratio: 1;
      object-position: top; 
    }
    & .card-bottom {
      padding-top: 5px;
      & p {
        font-size: 1rem;
        text-transform: uppercase;
      }
    }
  }
}
</style>