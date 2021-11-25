<template>
    <header id="jumbo-container">
        <img src="../assets/img/jumbotron.jpg" alt="">
    </header>
</template>

<script>
export default {
  name: 'Jumbotron',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    #jumbo-container {
        // background-image: url("../assets/img/jumbotron.jpg");
        height: 40vh;
        object-fit: cover;
        overflow: hidden;
        
        img {
            width: 100%; 
        } 
    }
</style>