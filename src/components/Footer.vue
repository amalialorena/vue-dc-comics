<template>
  <footer>
      <section class="content container">
          <div class="links">
                <ul>
                  <li>
                      <a href="#" class="title">DC COMICS</a>
                      <p>lorem</p>
                      <p>lorem</p>
                      <p>lorem</p>
                      <p>lorem</p>
                      <p>lorem</p>
                      <p>lorem</p>
                  </li>
                  <li><a href="#" class="title">COMICS</a>
                      <p>lorem</p>
                      <p>lorem</p>
                    </li>
                </ul>
                <ul>
                    <li><a href="#" class="title">DC</a>
                      <p>lorem</p>
                      <p>lorem</p>
                      <p>lorem</p>
                      <p>lorem</p>
                      <p>lorem</p>
                      <p>lorem</p>
                      <p>lorem</p>
                      <p>lorem</p>
                      <p>lorem</p>
                  </li>
                </ul>    
                <ul>
                    <li>
                      <a href="#" class="title">DC</a>
                      <p>lorem</p>
                      <p>lorem</p>
                      <p>lorem</p>
                  </li>
                </ul>  
    
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
                    height: 500px;
                }
            }
            .links {
                display: flex;
                justify-content: space-between;
                width: 30%;
                padding-top: 50px;
                ul a {
                    text-decoration: none;
                }
                 ul li .title {
                     color: white;
                     margin: 10px 0;
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
                }
            }

            .social {
                display:flex;
                align-items: center;
                p{
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