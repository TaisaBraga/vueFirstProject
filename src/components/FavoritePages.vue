<template>
  <div class="favorite-pages">
    <h2>Favorite Pages</h2>
    <ul>
      <li 
      v-for="page of favoritePages" 
      v-bind:key="page.id">
        <a :href="page.link">{{ page.nome }}</a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'FavoritePages',
  data(){
    return {
      favoritePages: []
    }
  },
  //criando o metodo para consumir a API
  created(){
    fetch('https://hackthon-decola.firebaseio.com/sites-favoritos.json') //criando a requisiçao
    .then(response => response.json()) // entao resultado e atribuir a json
    .then(json => { //json atribuir ao favoritePages
      this.favoritePages = json
      
    })
  }
}
</script>

<style scoped>

</style>
