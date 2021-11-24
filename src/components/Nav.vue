<template>
  <nav>
      <div class="container">
          <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="logo">
         </div>
            <ul>
                <li>
                    <a href="#">Character</a>
                </li>
                <li>
                    <a href="#">Character</a>
                </li>
                <li>
                    <a href="#">Character</a>
                </li>
                <li>
                    <a href="#">Character</a>
                </li>
                <li>
                    <a href="#">Character</a>
                </li>
            </ul>
      </div>
  </nav>

</template>

<script>
export default {
  name: 'Nav',  
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
        li {
            // vertical-align: middle;
            display: inline-block;
            margin: 0 20px;
            line-height: 70px;
            a {
                text-decoration: none;
            }
        }
    }
</style>
