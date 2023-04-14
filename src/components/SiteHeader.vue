

<script>
export default{
    name: 'SiteHeader',
    data(){
        return{
            menù: [
            {
                text: 'CHARACTERS',
                href: '#',
                currentPage: true
            },
            {
                text: 'characters',
                href: '#',
                currentPage: false
            },
            {
                text: 'characters',
                href: '#',
                currentPage: false
            },
            {
                text: 'characters',
                href: '#',
                currentPage: false
            },
            {
                text: 'characters',
                href: '#',
                currentPage: false
            },
            {
                text: 'characters',
                href: '#',
                currentPage: false
            },
            {
                text: 'characters',
                href: '#',
                currentPage: false
            },
            {
                text: 'characters',
                href: '#',
                currentPage: false
            },
            {
                text: 'characters',
                href: '#',
                currentPage: false
            },
            {
                text: 'characters',
                href: '#',
                currentPage: false
            }
            ]
        }
    }
}
</script>

<template>
    
  <header class="my-2">
    <nav class="container">
      <div class="row">
        <div class="col">
          <img src="../assets/img/dc-logo.png" alt="DC" class="mt-2">
        </div>
        <div class="col">
          <ul class="d-flex gap-3 mt-5">
            <li v-for="text in menù">{{ text.text }}</li>
    
          </ul>
        </div>
      </div>

    </nav>
  </header>
</template>

<style lang="scss" scoped>
      header{
    
    li{
      list-style-type: none;
      font-weight: 600;
    }
  }
</style>