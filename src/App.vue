<template>
  <div id="app">
    <IfTest/>
    <ForTest/>
    <EventTest/>
    <FavoritePages/>
  </div>
</template>

<script>
import IfTest from './components/IfTest'
import ForTest from './components/ForTest'
import EventTest from './components/EventTest'
import FavoritePages from './components/FavoritePages'

export default {
  name: 'App',
  components: {
    IfTest,
    ForTest,
    EventTest,
    FavoritePages
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
