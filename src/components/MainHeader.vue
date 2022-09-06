<template >
  <header class="container">
    <div class="logo">
      <img :src="logo.src" :alt="logo.alt">
    </div>
    <nav class="main-nav">
      <ul>
        <li v-for="(link, index) in navLinksArray" :class="link.current ? 'active' : ''"  :key="index" class="nav-link">
          <a :href="link.href">{{link.name}}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>
<script>
  import src from '../assets/img/dc-logo.png'
  
  export default{
    name : 'MainHeader',
    data () {
      return {
        logo:{
          src:src,
          alt: 'logo dc',
        }, 
        navLinksArray : [
          {
            href: '#',
            name: 'CHARACTERS',
            current: false,

          },
          {
            href: '#',
            name: 'COMICS',
            current: false,

          },
          {
            href: '#',
            name: 'MOVIES',
            current: false,

          },
          {
            href: '#',
            name: 'TV',
            current: false,

          },
          {
            href: '#',
            name: 'GAMES',
            current: false,

          },
          {
            href: '#',
            name: 'COLLECTIBLES',
            current: false,

          },
          {
            href: '#',
            name: 'VIDEOS',
            current: false,

          },
          {
            href: '#',
            name: 'FANS',
            current: false,

          },
          {
            href: '#',
            name: 'NEWS',
            current: false,

          },
          {
            href: '#',
            name: 'SHOP',
            current: false,

          },

        ]
      }
    }
    
  }
</script>
<style scoped lang="scss">
  @import '../styles/index.scss';
  @import '../styles/variables';
  header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    
      .main-nav{
        
        ul {
          display: flex;
          justify-content: space-between;
          align-items: center;
          height: 150px;
          gap: 15px;
          .nav-link {
            font-weight: 600;
            position: relative;
            display: flex;
            align-items: center;
            height: 100%;
            
          
            &.active, &:hover{
                color: $my-blue;
              }
            &.active::after, &:hover::after{
              content: "";
              height: 5px;
              background-color: $my-blue;
              width: 100%;
              display: block;
              position: absolute;
              bottom: 0;
              

              
            }  
          }
        }
      }
  }
  </style>