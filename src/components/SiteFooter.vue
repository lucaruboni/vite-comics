<script>
export default{
        name: 'SiteFooter',
        data(){

        }
    }
</script>

<template>
     <footer>
      <div class="row flex-wrap">
        <div class="col-12 up_col">
          <div class="container">
            <div class="row mt-5">
              <div class="col">
                <h2>DC COMICS</h2>
              
              <ul>
                <li>Characters</li>
                <li>Comics</li>
                <li>Movies</li>
                <li>TV</li>
                <li>Games</li>
                <li>Videos</li>
                <li>News</li>
                
              </ul>
              <h2>SHOP</h2>

                <ul>
                <li>Shop DC</li>
                <li>Shop DC Collectibles</li>
                </ul>

              </div>  
              <div class="col">
                <h2>DC</h2>
              
              <ul>
                <li>Terms of Use</li>
                <li>Privacy policy</li>
                <li>Ad Choices</li>
                <li>Advertising</li>
                <li>Jobs</li>
                <li>Subscription</li>
                <li>Talent Workshops</li>
                <li>CPSC Certificates</li>
                <li>Ratings</li>
                <li>Shop Help</li>
                <li>Contact Us</li>
                
              </ul>
            

              </div> 
              <div class="col">
                <h2>SITES</h2>
              
              <ul>
                <li>DC</li>
                <li>MAD Magazine</li>
                <li>DC Kids</li>
                <li>DC Universe</li>
                <li>DC Power Visa</li>
                
              </ul>
             

              </div> 
              
              <div class="col">
                <img src="../assets/img/dc-logo-bg.png" alt="logo-bg" class="logo_back">
              </div>
            
            </div>
          </div>
        </div>
        <div class="col down_col d-flex justify-content-between">
          
          <div class="container">
            <div class="row">
              <div class="col d-flex">
            <button type="button" class="btn my_btn btn-outline-primary align-self-center">SIGN-UP NOW!</button>
          </div>
          
          <div class="col d-flex py-5 gap-3">
            <h3 class="me-4">FOLLOW US</h3>
            <img src="../assets/img/footer-facebook.png" alt="">
            <img src="../assets/img/footer-periscope.png" alt="">
            <img src="../assets/img/footer-pinterest.png" alt="">
            <img src="../assets/img/footer-twitter.png" alt="">
            <img src="../assets/img/footer-youtube.png" alt="">
          </div>

            </div>
          </div>
          
        </div>
      </div>
    
  </footer>
</template>

<style lang="scss" scoped>

footer{
   
   height: 450px;

   h3{
     color: #0282f9;
   }

   ul{
     padding-left: 0;
   }
   li{
     list-style-type: none;
     color: grey;
     font-size: 0.9rem;
   }
   .logo_back{
     height: 400px;
    
   }
   .row{
     color: white;
   .up_col{
     
     background-image: url(../assets/img/footer-bg.jpg);
     background-repeat: no-repeat;
     background-size: cover;
   }
   .down_col{
     background-color: #303030;
    
     .my_btn{
       color: white;
       border-radius: 0;
       border-width: 2px;
       padding-bottom: 12px;
       padding-top: 12px;
       font-weight: 600;
     }
   }
  }
 }

</style>