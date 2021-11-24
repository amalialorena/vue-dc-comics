<template>
  <section>
      <div class="container">
          <div class="card" v-for="(card, i) in cards" :key="i">
              <img :src="require(`../assets/img/${card.image}`)" alt="" />
              <p>{{card.text}}</p>
          </div>
      </div>
  </section>
</template>

<script>
export default {
  name: 'Shop', 
  data() {
      return {
        cards:[
            {
            "text": "Digital Comics",
            "image": "buy-comics-digital-comics.png"
            },
            {
            "text": "DC Merchandise",
            "image": "buy-comics-merchandise.png"
            },
            {
            "text": "Subscriptions",
            "image": "buy-comics-subscriptions.png"
            },
            {
            "text": "Comic Shop Locator",
            "image": "buy-comics-shop-locator.png"
            },
            {
            "text": "DC Power Visa",
            "image": "buy-dc-power-visa.svg"
            },
        ]
      }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    section {
        background-color: #3069f7;
        color: white;
        height: 120px;

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 100%;
                .card {
                    display: flex;
                    align-items: center;
                    margin: 0 10px;
                    height: 50%;
                    width: calc((100% / 5) - 20px);
                    img {
                        width: 20%;
                        min-width: 30px;
                     }
                    p {
                        display: inline-block;
                        font-size: .8em;
                        margin: 0 10px;
                        vertical-align: middle;
                        font-weight: bold;
                    }
                }
           
        }
    
    }



</style>