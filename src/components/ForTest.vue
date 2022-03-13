<template>
<div class="for-test">
  <h2>For Test</h2>
  <ul>
    <li v-for="animal of animals" v-bind:key="animal.id"> <!--diretiva v-for-->
     <!--diretiva v-bind-key, para identificacao dos elementos dos array no JS-->
      <img v-bind:src="animal.url" v-bind:alt="animal.name"><!--diretiva v-bind para o HTML ler o codigo que vem do JS-->
    </li>
  </ul>
</div>

</template>

<script>

export default {
  name: 'ForTest',

  data(){
    return {
      animals: [
        {
          id: 1, //identificaçao do elemento
          name: 'little cat',
          url: 'https://www.petz.com.br/blog/wp-content/uploads/2020/04/meu-primeiro-gato.jpg'
        },
        {
          id: 2,
          name: 'little dog',
          url: 'https://image.cachorrogato.com.br/thumb/1200/630/1/imagens/original/imagem858.jpg'
        },
        {
          id: 3,
          name: 'test element',
          url: 'https://cdn.pixabay.com/photo/2017/06/05/07/58/butterfly-2373175_960_720.png'
        },
        {
          id: 4,
          name: 'mundi map',
          url: 'https://cdn.pixabay.com/photo/2017/06/14/08/20/map-of-the-world-2401458_960_720.jpg'
        }
      ]
    }
    
  }
}

</script>

<style scoped>
</style>