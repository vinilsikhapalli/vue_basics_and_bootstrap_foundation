<template>
  <div id="app">
   <BootstrapFondation/>
  </div>
</template>

<script>
import BootstrapFondation from './components/BootstrapFondation'

export default {
  name: 'App',
  components: {
    BootstrapFondation
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
