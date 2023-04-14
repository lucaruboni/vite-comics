<script>
import comics from './data/dc-comics.json'
export default{
    name: 'SiteMain',
    data(){
        return{
            comics: comics
        }
    }
}
</script>

<template>
    <main>
    <h1>     --> Your content goes here!</h1>
  </main>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables.scss' as *;

main{
  height: 180px;
  background-color: $darker;
  h1{
    color: $light;
    padding-top: 2rem;
  }
}

</style>