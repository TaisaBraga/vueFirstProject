<template>
  <div class="event-test">
    <h2>Event Test</h2>
    <!--interpolação, o que estiver dentro das 2 chaves, vai ser exibido no browser com logica-->
    <!--evento de passar o mouse, inserido pelo metodo criado no script-->
    <p v-on:mouseover="setUpperCase">{{ mensagem }}</p> 
  </div>
</template>

<script>

export default {
  name: 'EventTest',
  data(){
    return {
      mensagem: 'O rato roeu a roupa do rei de roma'
    }
  }, 
  methods: { //metodo para colocar a mensagem em Upper Case
    setUpperCase() {
      this.mensagem = this.mensagem.toUpperCase();
    }
  }
}
</script>

<style scoped>
</style>
