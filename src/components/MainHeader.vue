<template >
  <header class="container">
    <div class="logo">
      <img src="../assets/img/dc-logo.png" alt="logo dc">
    </div>
    <nav class="main-nav">
      <ul>
        <li class="nav-link">
          <a href="#">CHARACTERS</a>
        </li>
        <li class="nav-link">
          <a href="#">COMICS</a>
        </li>
        <li class="nav-link">
          <a href="#">MOVIES</a>
        </li>
        <li class="nav-link">
          <a href="#">TV</a>
        </li>
        <li class="nav-link">
          <a href="#">GAMES</a>
        </li>
        <li class="nav-link">
          <a href="#">COLLECTIBLES</a>
        </li>
        <li class="nav-link">
          <a href="#">VIDEOS</a>
        </li>
        <li class="nav-link">
          <a href="#">FANS</a>
        </li>
        <li class="nav-link">
          <a href="#">NEWS</a>
        </li>
        <li class="nav-link">
          <a href="#">SHOP</a>
        </li>
      </ul>
    </nav>
  </header>
</template>
<script>
  
  export default{
    name : 'MainHeader'
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
            &:hover::after{
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