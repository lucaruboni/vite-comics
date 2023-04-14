<script>
import comics from './data/dc-comics.json'
import ComicsItem from './ComicsItem.vue'
export default{
    name: 'SiteMain',
    components: {
        ComicsItem 
    },
    data(){
        return{
            comics: comics
        }
    }
}
</script>

<template>
    <div class="banner">
       
    </div>

    

    <main>
   <!--  <h1>    Your content goes here!</h1> -->
        
        

   <div class="container">
        <div class="row justify-content-center position-relative">

            <button id="my_btn_position" class="btn btn-primary main_btn">CURRENT SERIES</button>

                <ul class="d-flex flex-wrap gap-4 mt-5">
                   
                        <ComicsItem :thumb="comic.thumb" :series="comic.series" v-for="comic in comics" />
                        
                    
                </ul>

                <button class="btn btn-primary main_btn my-5">LOAD MORE</button>
               
        </div>
    </div>






  </main>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables.scss' as *;


.banner{
    height: 450px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}

main{
  
  background-color: $darker;
  h1{
    color: $light;
    padding-top: 2rem;
  }

  .main_btn{
    width: 200px;
    height: 60px;
    font-weight: 600;
    border-radius: 0;
  }
  #my_btn_position{
    width: 250px;
    height: 70px;
    position: absolute;
    top: -35px;
    left: 12px;
    font-size: 1.6rem;
    font-weight: 900;

  }
   
}

</style>