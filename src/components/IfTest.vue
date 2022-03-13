<template>
<div class="if-test">
  <h1 v-if='canSee'>Test One</h1> <!--Se TRUE-->
  <h1 v-else>Test</h1> <!--Se FALSE-->
 
</div>
</template>

<script>

export default {
  name: 'IfTest',
  //Dentro de data() estão os dados que serão utilizados do próprio componente.
  data (){
    return {
      canSee: true //criando a função de condição
    }
  }
}

</script>
<style scoped></style>
