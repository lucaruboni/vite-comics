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
        <div class="row">
                <ul class="d-flex flex-wrap gap-5">
                   
                        <ComicsItem :thumb="comic.thumb" :series="comic.series" v-for="comic in comics" />
                        
                    
                </ul>
               
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

 
}

</style>