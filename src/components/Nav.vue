<template>
  <nav>
      <div class="container">
          <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="logo">
         </div>
            <ul>
                <li v-for="(link, i) in links" :key="i" :class="link.status? 'active' : ''">
                    <a href="#">{{link.text.toUpperCase()}}</a>
                </li>
            </ul>
      </div>
  </nav>

</template>

<script>
export default {
  name: 'Nav',  
  data() {
      return {
          links:[
              {
                  text:"characters",
                  status: false
              },
              {
                  text:"comics",
                  status: true
              },
              {
                  text:"movies",
                  status: false
              },
              {
                  text:"tv",
                  status: false
              },
              {
                  text:"games",
                  status: false
              },
              {
                  text:"collectibles",
                  status: false
              },
              {
                  text:"videos",
                  status: false
              },
              {
                  text:"fans",
                  status: false
              },
              {
                  text:"news",
                  status: false
              },
              {
                  text:"shop",
                  status: false
              }
              
            ]
      }
  }

  

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    nav {
        .container {
            height: 70px;
            display: flex;
            justify-content: space-between;
        }
        .logo {
            padding: 5px;
        }
        img {
            height: 100%;
        }
        .active a {
            color: blue;
            border-bottom:  3px solid blue;
            padding-bottom: 25px;
        }
        li {
            display: inline-block;
            margin: 0 10px;
            line-height: 70px;
            a {
                text-decoration: none;
                font-size: .7em;
                color: black;
                font-weight: bold;
            }
        }
    }
</style>
