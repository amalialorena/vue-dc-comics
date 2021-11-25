<template>
  <div class="card">
      <div class="img-container">
          <img :src="img" alt="">
      </div>
      <p>{{title.toUpperCase()}}</p>
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
        width: calc((100% / 6) - 20px);
        margin: 20px 10px;
        .img-container {
            height: 180px;
            overflow: hidden;
            img {
            width: 100%;
            // min-height: 200px;
            }
        }
        
        p {
            margin-top: 15px;
            color: white;
            font-size: .7em;
            font-weight: bold;
        }
    }
</style>