<script>
export default{
    name: 'SiteSection',
    data(){
        return{
            banner: [
                {
                    text: 'DIGITAL COMICS',
                    src: 'buy-comics-digital-comics.png'
                },
                {
                    text: 'DC MERCHANDISE',
                    src: 'buy-comics-merchandise.png'
                },
                {
                    text: 'SUBSCRIPTION',
                    src: 'buy-comics-shop-locator.png'
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    src: 'buy-comics-subscriptions.png'
                },
                {
                    text: 'DC POWER VISA',
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
@use '../assets/scss/partials/variables.scss' as *;

  section{
    
    background-color: $primary;
    height: 105px;


    .col{
        margin: 2px;
        &:hover{
            border: 2px solid $light;
        }
    }
    
  
    img{
     
      height: 100px;
      align-self: center;
      
      }
    
    p{
      color: $light;
      font-size: 0.8rem;
      align-self: center;
      padding-top: 0.5rem;
    }
  }

</style>