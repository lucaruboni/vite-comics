import SiteHeader
<script>
  import SiteHeader from './components/SiteHeader.vue'
  import SiteSection from './components/SiteSection.vue'
  import SiteFooter from './components/SiteFooter.vue'
  export default{
    components : {
      SiteHeader,
      SiteSection,
      SiteFooter
    },

    data(){
      return{
        
      }
    }
  }

</script>

<template>
<SiteHeader/>

  <main>
    <h1>     --> Your content goes here!</h1>
  </main>
<SiteSection/>


<SiteFooter/>

</template>

<style lang="scss" scoped>
  
@use './assets/scss/partials/variables.scss';

  main{
    height: 180px;
    background-color: black;
    h1{
      color: white;
      padding-top: 2rem;
    }
  }






</style>