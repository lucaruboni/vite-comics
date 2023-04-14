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
     <li class="mt-3">
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
    
    height: 200px;
  }
  li{
    list-style-type: none;
    color: $light_dark;
  }

</style>