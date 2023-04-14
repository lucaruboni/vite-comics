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
                <li><a href="#">Characters</a> </li>
                <li><a href="#">Comics</a> </li>
                <li><a href="#">Movies</a> </li>
                <li><a href="#">TV</a> </li>
                <li><a href="#">Games</a> </li>
                <li><a href="#">Videos</a> </li>
                <li><a href="#"> News</a></li>
                
              </ul>
              <h2>SHOP</h2>

                <ul>
                <li><a href="#"> Shop DC</a></li>
                <li><a href="#">Shop DC Collectibles</a> </li>
                </ul>

              </div>  
              <div class="col">
                <h2>DC</h2>
              
              <ul>
                <li><a href="#"> Terms of Use</a></li>
                <li><a href="#"> Privacy policy</a></li>
                <li><a href="#"> Ad Choices</a></li>
                <li><a href="#"> Advertising</a></li>
                <li><a href="#"> Jobs</a></li>
                <li><a href="#"> Subscription</a></li>
                <li><a href="#"> Talent Workshops</a></li>
                <li><a href="#"> CPSC Certificates</a></li>
                <li><a href="#"> Ratings</a></li>
                <li><a href="#">Shop Help</a> </li>
                <li><a href="#">Contact Us</a> </li>
                
              </ul>
            

              </div> 
              <div class="col">
                <h2>SITES</h2>
              
              <ul>
                <li><a href="#"> DC</a></li>
                <li><a href="#"> MAD Magazine</a></li>
                <li><a href="#">DC Kids</a> </li>
                <li><a href="#">DC Universe</a> </li>
                <li><a href="#">DC Power Visa</a> </li>
                
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
@use '../assets/scss/partials/variables.scss' as *;

footer{
   
   height: 450px;

   h3{
     color: $primary;
   }

   ul{
     padding-left: 0;
   }
   li{
     list-style-type: none;
     color: $light_dark;
     font-size: 0.9rem;

     a{
        text-decoration: none;
        color: $light_dark;

        &:hover{
            color: $light;
            font-size: 1rem;
        }
     }
   }
   .logo_back{
     height: 400px;
    
   }
   .row{
     color: $light;
   .up_col{
     
     background-image: url(../assets/img/footer-bg.jpg);
     background-repeat: no-repeat;
     background-size: cover;
   }
   .down_col{
     background-color: $dark;
    
     .my_btn{
       color: $light;
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