<template >
  <footer>
    <div class="footer-pt-1">
      <div class="container">
        <ul>
          <li v-for="(item, index) in footerLinks1" :key="index">
            <a :href="item.href">
              <div>
                <img :src="item.src" :alt="item.alt">
              </div>
              <div>
                {{item.title}}
              </div>
            </a>
          </li>


        </ul>
      </div>
    </div>
    <div class="footer-pt-2">
      <div class="container">
        <div class="wrapper">
          <FooterList :title="titolo1" :links="menu1"/>
          <FooterList :title="titolo2" :links="menu2"/>
          <FooterList :title="titolo3" :links="menu3"/>
          <FooterList :title="titolo4" :links="menu4"/>




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
            <li v-for="(link, index) in footerLinks2" :key="index"><a :href="link.href"><img :src="link.src" :alt="link.alt"></a></li>
          </ul>
        </nav>
      </div>
    </div>
  </footer>
</template>
<script>
import FooterList from './FooterList.vue';
export default {
    name: "MainFooter",
    data() {
        return {
            footerLinks1: [
                {
                    href: "#",
                    src: require("../assets/img/buy-comics-digital-comics.png"),
                    alt: "logo digital comics",
                    title: "DIGITAL COMICS"
                },
                {
                    href: "#",
                    src: require("../assets/img/buy-comics-merchandise.png"),
                    alt: "logo dc merchandise",
                    title: "DC MERCHANDISE"
                },
                {
                    href: "#",
                    src: require("../assets/img/buy-comics-subscriptions.png"),
                    alt: "logo subscription",
                    title: "SUBSCRIPTION"
                },
                {
                    href: "#",
                    src: require("../assets/img/buy-comics-subscriptions.png"),
                    alt: "logo comic shop locator",
                    title: "COMIC SHOP LOCATOR"
                },
                {
                    href: "#",
                    src: require("../assets/img/buy-dc-power-visa.svg"),
                    alt: "logo dc power visa",
                    title: "DC POWER VISA"
                },
            ],
            titolo1: "DC COMICS",
            titolo2: "SHOP",
            titolo3: "DC",
            titolo4: "SITES",
            menu1: [
                {
                    href: "#",
                    text: "Characters",
                },
                {
                    href: "#",
                    text: "Comics",
                },
                {
                    href: "#",
                    text: "Movies",
                },
                {
                    href: "#",
                    text: "TV",
                },
                {
                    href: "#",
                    text: "Games",
                },
                {
                    href: "#",
                    text: "Videos",
                },
                {
                    href: "#",
                    text: "News",
                },
            ],
            menu2: [
                {
                    href: "#",
                    text: "Shop DC",
                },
                {
                    href: "#",
                    text: "Shop DC Collectibles",
                },
            ],
            menu3: [
                {
                    href: "#",
                    text: "Terms Of Use",
                },
                {
                    href: "#",
                    text: "Privacy Policy",
                },
                {
                    href: "#",
                    text: "Ad Choices",
                },
                {
                    href: "#",
                    text: "Advertising",
                },
                {
                    href: "#",
                    text: "Jobs",
                },
                {
                    href: "#",
                    text: "Subscriptions",
                },
                {
                    href: "#",
                    text: "Talent Workshops",
                },
                {
                    href: "#",
                    text: "CPSC Certificates",
                },
                {
                    href: "#",
                    text: "Ratings",
                },
                {
                    href: "#",
                    text: "Shop Help",
                },
                {
                    href: "#",
                    text: "Contact Us",
                },
            ],
            menu4: [
                {
                    href: "#",
                    text: "DC",
                },
                {
                    href: "#",
                    text: "Mad Magazine",
                },
                {
                    href: "#",
                    text: "DC Kids",
                },
                {
                    href: "#",
                    text: "DC Universe",
                },
                {
                    href: "#",
                    text: "DC Power Visa",
                },
            ],
            footerLinks2: [
              {
                href:'#',
                src: require("../assets/img/footer-facebook.png"),
                alt:'logo facebook',
              },
              {
                href:'#',
                src: require("../assets/img/footer-twitter.png"),
                alt:'logo twitter',
              },
              {
                href:'#',
                src: require("../assets/img/footer-youtube.png"),
                alt:'logo youtube',
              },
              {
                href:'#',
                src: require("../assets/img/footer-pinterest.png"),
                alt:'logo pinterest',
              },
              {
                href:'#',
                src: require("../assets/img/footer-periscope.png"),
                alt:'logo periscope',
              },
            ]
        };
    },
    components: { FooterList }
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

  & .container {
    display: flex;
    position: relative;
    height: 450px;


    & .logo-big {
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


      

    }

  }


}

footer .footer-pt-3 {
  position: relative;
  z-index: 2;
  background-color: rgb(39, 37, 37);
  padding: 30px 0;

  & .container {
    display: flex;
    justify-content: space-between;
    align-items: center;

    & button {
      display: inline-block;
      padding: 8px;
      border: 4px solid $my-blue;
      color: white;
      background-color: transparent;
      font-size: 1.5rem;
    }

    & .social-links {
      display: flex;
      gap: 30px;
      align-items: center;

      &>a {
        color: $my-blue;
        font-size: 1.5rem;
        font-weight: 600;
      }

      & ul {
        display: flex;
        justify-content: space-between;
        gap: 20px;
        align-items: center;
      }

    }

  }
}
</style>