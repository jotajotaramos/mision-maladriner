<template>
  <SheepCounter msg="Welcome to Your Sheep Counter App"/>
</template>

<script>
import SheepCounter from './components/SheepCounter.vue'

export default {
  name: 'App',
  components: {
    SheepCounter
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
