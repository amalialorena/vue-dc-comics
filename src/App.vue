<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Nav/>
    <main>
    
    </main>
    <Shop/>
    <Footer/>
  </div>
</template>

<script>
import Nav from './components/Nav.vue';
import Shop from './components/Shop.vue';
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    Nav,
    Shop,
    Footer
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
