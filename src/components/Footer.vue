<template>
  <footer>
      <section class="content container">
          <div class="links">
              <div class="column"> 
                <ul>
                  <li v-for="(product,i) in products" :key="i">
                      <a :href="product.link" :class="i===0? 'title': '' ">{{product.text}}</a>
                  </li>
                  </ul>
                  <ul>
                  <li v-for="(shop,i) in shops" :key="i">
                      <a href="shop.link" :class="i===0? 'title': ''">{{shop.text}}</a> 
                  </li>
                </ul>
              </div>
              <div class="column">  
                <ul>
                    <li v-for="(object,i) in legal" :key="i">
                      <a href="object.link" :class="i===0? 'title': ''">{{object.text}}</a>
                  </li>
                </ul>    
              </div>
              <div class="column">
                <ul>
                    <li v-for="(site,i) in sites" :key="i">
                      <a href="site.link" :class="i===0? 'title': ''">{{site.text}}</a>
                  </li>
                </ul>  
            </div>
          </div> 
          <div class="logo">
              <img src="../assets/img/dc-logo-bg.png" alt="">
          </div>
      </section>
      <section class="social-container">
          <div class="container">
                <button>SIGN UP NOW</button>
                <div class="social">
                    <p>FOLLOW US</p> 
                    <img src="../assets/img/footer-facebook.png" alt=""> 
                    <img src="../assets/img/footer-twitter.png" alt="">
                    <img src="../assets/img/footer-youtube.png" alt=""> 
                    <img src="../assets/img/footer-pinterest.png" alt=""> 
                    <img src="../assets/img/footer-periscope.png" alt=""> 
                </div>
          </div>
      </section>
  </footer>
</template>

<script>
export default {
  name: 'Footer', 
  data () {
      return {
          products: [
            { 
               text: "DC COMICS",
               link: "#"
            },
             { 
               text:  "Characters",
               link: "#"
            },
            { 
               text:  "Comics",
               link: "#"
            }, 
            { 
               text:  "Movies",
               link: "#"
            }, 
            { 
               text:  "Tv",
               link: "#"
            },
            { 
               text: "Games",
               link: "#"
            },
            { 
               text: "Videos",
               link: "#"
            }, 
            { 
               text: "News",
               link: "#"
            }, 
          ],
          shops: [
            { 
               text: "Shop DC", 
               link: "#"
            },
            { 
               text: "SHOP",
               link: "#"
            },
            { 
               text: "Shop Collectibles",
               link: "#"
            }, 
          ],
          legal: [
            { 
               text: "DC",
               link: "#"
            },
            { 
               text: "Terms of use",
               link: "#"
            },
            { 
               text: "Add Choices",
               link: "#"
            },
            { 
               text: "Advertising",
               link: "#"
            },
            { 
               text: "Jobs",
               link: "#"
            },
            { 
               text: "Subscriptions",
               link: "#"
            },
            { 
               text: "CPSC Certificates",
               link: "#"
            },
            { 
               text: "Ratings",
               link: "#"
            },
            { 
               text: "Shop Help",
               link: "#"
            },
            { 
               text: "Contact Us",
               link: "#"
            },            
          ],
          sites: [
            { 
               text: "SITES",
               link: "#"
            },
            { 
               text: "MAD Magazine",
               link: "#"
            },
            { 
               text: "DC Kids",
               link: "#"
            },
            { 
               text: "DC Universe",
               link: "#"
            },
            { 
               text: "DC Power Visa",
               link: "#"
            },       
          ]
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    footer{
        background-image: url("../assets/img/footer-bg.jpg");
        background-size: cover;
        background-position: center;
        .content {
            display: flex;
            justify-content: space-between;
            height: 350px;
            .logo {
                width: 50%;
                overflow: hidden;
                object-fit: cover;
                img {
                    max-width: 100%;
                    margin-top: -70px;
                }
            }
            .links {
                display: flex;
                justify-content: space-between;
                width: 30%;
                padding-top: 50px;
                color:grey;

                ul a {
                    text-decoration: none;
                    font-size: .7em;
                    color: grey;
                }
                .title {
                    color: white;
                    margin: 10px 0;
                    font-weight: bold;
                    font-size: .9em;
                    display: block;
                }
                
            }
            
        }
        
        .social-container {
            background-color: #242424;

            .container {
                display:flex;
                justify-content: space-between;
                height: 100px;
                button {
                    border: 1px solid #0c6bfb;
                    margin: 30px;
                    background-color: #242424;
                    color: white;
                    place-self: center;
                    padding: 10px;
                }
            }

            .social {
                display:flex;
                align-items: center;
                p {
                    display: inline-block;
                    color:#0c6bfb;
                    font-weight: bold;
                    margin-right: 10px;
                }

                img {
                    margin: 10px;
                }
            }
        }
    }

</style>