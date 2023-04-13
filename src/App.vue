<script>
   
  export default{

  }

</script>

<template>

  <header>
    <nav class="container">
      <div class="row">
        <div class="col">
          <img src="./assets/img/dc-logo.png" alt="DC" class="mt-3">
        </div>
        <div class="col">
          <ul class="d-flex gap-3 mt-5">
            <li>CHARACTERS</li>
            <li>COMICS</li>
            <li>MOVIES</li>
            <li>TV</li>
            <li>GAMES</li>
            <li>COLLECTIBLES</li>
            <li>VIDEO</li>
            <li>FANS</li>
            <li>NEWS</li>
            <li>SHOP</li>
          </ul>
        </div>
      </div>

    </nav>
  </header>

  <main>
    <h1>     --> Your content goes here!</h1>
  </main>

  <section>
    <div class="container"></div>
    <div class="row mx-5">
      <div class="col">
        <img src="./assets/img/buy-comics-digital-comics.png" alt="buy comics" class="p-4">
      </div>
      
      <div class="col">
        <img src="./assets/img/buy-comics-merchandise.png" alt="buy comics" class="p-4">
      </div>

      <div class="col">
        <img src="./assets/img/buy-comics-shop-locator.png" alt="buy comics" class="p-4">
      </div>

      <div class="col">
        <img src="./assets/img/buy-comics-subscriptions.png" alt="buy comics" class="p-4">
      </div>

      <div class="col">
        <img src="./assets/img/buy-dc-power-visa.svg" alt="buy comics" class="p-4">
      </div>
      
    </div>
  </section>

  <footer>
      <div class="row flex-wrap">
        <div class="col-12 up_col">

        </div>
        <div class="col down_col"></div>
      </div>
    
  </footer>

</template>

<style lang="scss" scoped>
  
  header{
    
    height: 150px;
    li{
      list-style-type: none;
    }
  }


  main{
    height: 180px;
    background-color: black;
    h1{
      color: white;
      padding-top: 2rem;
    }
  }



  section{
    height: 180px;
    background-color: blue;
    img{
     margin-top: 2rem;
      height: 100px;
    }
  }



  footer{
   
    height: 450px;
    
    .row{
    
    .up_col{
      height: 350px;
      background-image: url(./assets/img/footer-bg.jpg);
      background-repeat: no-repeat;
      background-size: cover;
    }
    .down_col{
      background-color: grey;
      height: 100px;
    }
   }
  }

</style>