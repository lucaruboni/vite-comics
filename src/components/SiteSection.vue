<script>
export default{
    name: 'SiteSection',
    data(){
        return{
            banner: [
                {
                    text: 'Digital Comics',
                    src: 'buy-comics-digital-comics.png'
                },
                {
                    text: 'Digital Comics',
                    src: 'buy-comics-merchandise.png'
                },
                {
                    text: 'Digital Comics',
                    src: 'buy-comics-shop-locator.png'
                },
                {
                    text: 'Digital Comics',
                    src: 'buy-comics-subscriptions.png'
                },
                {
                    text: 'Digital Comics',
                    src: 'buy-dc-power-visa.svg'
                }
                
            ]
        }
    },
    methods: {
        getImageUrl(name) {
            return new URL(`../assets/img/${name}`, import.meta.url).href
        }
    }
}

</script>

<template>
    <section>
    <div class="container">
    <div class="row mx-5">
      <div class="col d-flex" v-for="item in banner">
        <img :src="getImageUrl(item.src)" alt="buy comics" class="p-4">
        <p>{{ item.text }}</p>
      </div>
      
<!--       <div class="col d-flex">
        <img src="./assets/img/buy-comics-merchandise.png" alt="buy comics" class="p-4">
        <p>DC MERCHANDISE</p>
      </div>

      <div class="col d-flex">
        <img src="./assets/img/buy-comics-shop-locator.png" alt="buy comics" class="p-4">
        <p>SUBSCRIPTION</p>
      </div>

      <div class="col d-flex">
        <img src="./assets/img/buy-comics-subscriptions.png" alt="buy comics" class="p-4">
        <p>COMIC SHOP LOCATOR</p>
      </div>

      <div class="col d-flex">
        <img src="./assets/img/buy-dc-power-visa.svg" alt="buy comics" class="p-4">
        <p>DC POWER VISA</p>
      </div> -->
      
    </div>
  </div>
  </section>
</template>

<style lang="scss" scoped>
  section{
    
    background-color: #0282f9;
    img{
     
      height: 100px;
      align-self: center;
    }
    p{
      color: white;
      font-size: 0.8rem;
      align-self: center;
      padding-top: 0.5rem;
    }
  }

</style>