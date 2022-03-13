<template>
  <div class="counter-method">
    <h2>Contador</h2>
    <p> Counter: {{counter}}</p>

    <!--
        METODO QUE EU UTILIZEI
      <button v-if="counter > 0" v-on:click="counter = counter - 1">-</button>
      <button v-on:click="counter = counter + 1">+</button> 
    --->

      <button v-on:click="minusOne" >-</button>
      <button v-on:click="plusOne">+</button> 
    
  </div>
</template>
<script>

export default {
  name: 'CountingNumbers',
  data() {
    return {
      counter: 0
    }
  },
  methods: {
    plusOne(){
      this.counter++
    },
    minusOne(){
      if(this.counter > 0) this.counter--
    }
  }
}
</script>
<style scoped>

</style>
