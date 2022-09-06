<template>
  <div class="col">
    <h3>{{title}}</h3>
    <ul>
      <li v-for="(link, index) in links" :key="index">
        <a :href="link.href">{{link.text}}</a>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: 'FooterList',
  props: {
    title: String,
    links: Array,
  },

}
</script>
<style scoped>
@import '../styles/index.scss';

  h3 {
    color: white;
    margin-bottom: 20px;
  }
  
  li {
    color: grey;
    line-height: 1.5rem;
  }
  
  li:hover {
    color: white;
  }


</style>