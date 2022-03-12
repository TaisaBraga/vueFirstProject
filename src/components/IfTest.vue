<template>
<div class="if-test">
  <h1 v-if='canSee'>test</h1>
 
</div>

</template>
<script>

export default {
  name: 'IfTest',
  //Dentro de data() estão os dados que serão utilizados do próprio componente.
  data (){
    return {
      canSee: true
    }
  }
}

</script>
<style scoped></style>
