<template>
  <div id="app">
    <IfTest/>
    <ForTest/>
    <EventTest/>
    <FavoritePages/>
    <CounterTest/>
  </div>
</template>

<script>
import IfTest from './components/IfTest'
import ForTest from './components/ForTest'
import EventTest from './components/EventTest'
import FavoritePages from './components/FavoritePages'
import CounterTest from './components/CounterTest'

export default {
  name: 'App',
  components: {
    IfTest,
    ForTest,
    EventTest,
    FavoritePages,
    CounterTest
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;

}
</style>
