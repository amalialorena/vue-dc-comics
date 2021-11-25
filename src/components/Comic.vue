<template>
  <div class="card">
        <img :src="img" alt="">
        <p>{{title}}</p>
  </div>
</template>

<script>
export default {
  name: 'Comic',
  
  props: {
    img: String, 
    title: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .card {
        width: calc((100% / 6) - 10px);
        margin: 5px;
    }
</style>