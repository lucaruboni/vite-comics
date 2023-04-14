<script>
export default{
    name: 'ComicsItem',
    props: {
        thumb: String,
        series: String
    }
}
</script>

<template>
     <li class="mt-3 d-flex">
        <div>
          <img :src="thumb" class="card-img-top" alt="...">
          <div>
            <p>{{ series }}</p>
          </div>
        </div>
    </li>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables.scss' as *;

img{
   max-width: 100%;
   max-height: 100%; 
   height: 400px;
   width: 300px;

   &:hover{
    filter: blur(1px);
   }
    
  }
  li{
   
    
    list-style-type: none;
    color: $light_dark;
     
    p{
        font-size: 0.9rem;
        margin-top: 5px;
    }

  }

</style>