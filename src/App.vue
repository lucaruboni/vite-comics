import SiteHeader
<script>
  import SiteHeader from './components/SiteHeader.vue'
  import SiteSection from './components/SiteSection.vue'
  import SiteFooter from './components/SiteFooter.vue'
  import SiteMain from './components/SiteMain.vue'
  
  export default{
    components : {
      SiteHeader,
      SiteSection,
      SiteFooter,
      SiteMain
    },

    data(){
      return{
        
      }
    }
  }

</script>

<template>
<SiteHeader/>
<SiteMain/>

<SiteSection/>


<SiteFooter/>

</template>

<style lang="scss" scoped>
  






</style>