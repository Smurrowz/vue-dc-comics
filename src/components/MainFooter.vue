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
  </footer>
</template>
<script>
  export default{
    name : 'MainFooter'
  }
</script>
<style scoped lang="scss">
  @import '../styles/index.scss';
  @import '../styles/variables';
  footer .footer-pt-1{
    background-color: $my-blue;
    padding: 50px 0;
    color: white;
    & ul{
      display: flex;
      justify-content: space-between;
      align-items: center;
      & a{
        display: flex;
        gap: 20px;
        align-items: center;
        justify-content: space-between;
        & img{
          height: 60px;
        }
      }
    }
  }
</style>