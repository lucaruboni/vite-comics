

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
                text: 'COMICS',
                href: '#',
                currentPage: false
            },
            {
                text: 'MOVIES',
                href: '#',
                currentPage: false
            },
            {
                text: 'TV',
                href: '#',
                currentPage: false
            },
            {
                text: 'GAMES',
                href: '#',
                currentPage: false
            },
            {
                text: 'COLLECTIBLES',
                href: '#',
                currentPage: false
            },
            {
                text: 'VIDEOS',
                href: '#',
                currentPage: false
            },
            {
                text: 'FANS',
                href: '#',
                currentPage: false
            },
            {
                text: 'NEWS',
                href: '#',
                currentPage: false
            },
            {
                text: 'SHOP',
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
@use '../assets/scss/partials/variables.scss' as *;
      header{
        position: sticky;
        top: 0;
        left: 0;
        height: 150px;

    li{
      list-style-type: none;
      font-weight: 600;
    }
  }
</style>