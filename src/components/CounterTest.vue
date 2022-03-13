<template>
  <div class="counter-method">
    <h2>Counter: {{counter}}</h2>
    <button v-if="counter > 0" v-on:click="counter = counter - 1">-</button>
    <button v-on:click="counter = counter + 1">+</button>
  </div>
</template>
<script>

export default {
  name: 'CountingNumbers',
  data() {
    return {
      counter: 0

    }
  }
}
</script>
<style scoped>

</style>
