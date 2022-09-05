<template >
  <footer>
    <div class="footer-pt-1">
      <div class="container">
        <ul>
          <li>
            <a href="#">
              <div>
                <img src="../assets/img/buy-comics-digital-comics.png" alt="logo digital comics">
              </div>
              <div>
                DIGITAL COMICS
              </div>
            </a>
          </li>
          <li>
            <a href="#">
              <div>
                <img src="../assets/img/buy-comics-merchandise.png" alt="logo digital comics">
              </div>
              <div>
                DC MERCHANDISE
              </div>
            </a>
          </li>
          <li>
            <a href="#">
              <div>
                <img src="../assets/img/buy-comics-subscriptions.png" alt="logo digital comics">
              </div>
              <div>
                SUBSCRIPTION
              </div>
            </a>
          </li>
          <li>
            <a href="#">
              <div>
                <img src="../assets/img/buy-comics-shop-locator.png" alt="logo digital comics">
              </div>
              <div>
                COMIC SHOP LOCATOR
              </div>
            </a>
          </li>
          <li>
            <a href="#">
              <div>
                <img src="../assets/img/buy-dc-power-visa.svg" alt="logo digital comics">
              </div>
              <div>
                DC POWER VISA
              </div>
            </a>
          </li>

        </ul>
      </div>
    </div>
    <div class="footer-pt-2">
      <div class="container">
        <div class="wrapper">
          <div class="col">
            <h3>DC COMICS</h3>
            <ul>
              <li><a href="#">Character</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>


          </div>
          <div class="col">
            <h3>SHOP</h3>
            <ul>
              <li><a href="#">Shop DC</a></li>
              <li><a href="#">Shop DC Collectibles</a></li>
            </ul>


          </div>
          <div class="col">
            <h3>DC</h3>
            <ul>
              <li><a href="#">Terms Of Use</a></li>
              <li><a href="#">Privacy Policy (New)</a></li>
              <li><a href="#">Ad Choices</a></li>
              <li><a href="#">Advertising</a></li>
              <li><a href="#">Jobs</a></li>
              <li><a href="#">Subscriptions</a></li>
              <li><a href="#">Talent Workshops</a></li>
              <li><a href="#">CPSC Certificates</a></li>
              <li><a href="#">Ratings</a></li>
              <li><a href="#">Shop Help</a></li>
              <li><a href="#">Contact Us</a></li>
            </ul>


          </div>
          <div class="col">
            <h3>SITES</h3>
            <ul>
              <li><a href="#">DC</a></li>
              <li><a href="#">MAD Magazine</a></li>
              <li><a href="#">DC Kids</a></li>
              <li><a href="#">DC Universe</a></li>
              <li><a href="#">DC Power Visa</a></li>
            </ul>


          </div>

        </div>
        <div>
          <img class="logo-big" src="../assets/img/dc-logo-bg.png" alt="">
        </div>
      </div>
    </div>
    <div class="footer-pt-3">
      <div class="container">
        <button>SIGN-UP NOW</button>
        <nav class="social-links">
          <a href="#"> FOLLOW US</a>
          <ul>
            <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="logo social"></a></li>
            <li><a href="#"><img src="../assets/img/footer-twitter.png" alt="logo social"></a></li>
            <li><a href="#"><img src="../assets/img/footer-youtube.png" alt="logo social"></a></li>
            <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt="logo social"></a></li>
            <li><a href="#"><img src="../assets/img/footer-periscope.png" alt="logo social"></a></li>
          </ul>
        </nav>
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  name: 'MainFooter'
}
</script>
<style scoped lang="scss">
@import '../styles/index.scss';
@import '../styles/variables';

footer .footer-pt-1 {
  background-color: $my-blue;
  padding: 50px 0;
  color: white;
  z-index: 2;
  position: relative;

  & ul {
    display: flex;
    justify-content: space-between;
    align-items: center;

    & a {
      display: flex;
      gap: 20px;
      align-items: center;
      justify-content: space-between;

      & img {
        height: 60px;
      }
    }
  }
}

footer .footer-pt-2 {
  background-image: url(../assets/img/footer-bg.jpg);
  background-size: cover;
  
  & .container{
    display: flex;
    position: relative;
    height: 450px;
    

    & .logo-big{
      position: absolute;
      z-index: 1;
      top: -40px;
      right: 0;
    }
    & .wrapper {
      display: flex;
      gap: 20px;
      flex-basis: 50%;
      padding: 40px 0;
      flex-direction: column;
      height: 100%;
      flex-wrap: wrap;
      
  
      & .col {
        
        & h3 {
          color: white;
          margin-bottom: 20px;
        }
    
        & ul {
    
          & li {
            color: grey;
            line-height: 1.5rem;
          }
        }
  
      }
  
    }

  }


}
footer .footer-pt-3 {
  position: relative;
  z-index:2;
  background-color: rgb(39, 37, 37);
  padding: 30px 0;
  & .container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    & button{
      display: inline-block;
      padding: 8px;
      border: 4px solid $my-blue;
      color: white;
      background-color: transparent;
      font-size: 1.5rem;
    }
    & .social-links{
      display: flex;
      gap: 30px;
      align-items: center;
      & > a{
        color: $my-blue;
        font-size: 1.5rem;
        font-weight: 600;
      }
      & ul{
        display: flex;
        justify-content: space-between;
        gap: 20px;
        align-items: center;
      }
      
    }

  }
}
</style>