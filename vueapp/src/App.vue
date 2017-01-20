<template>
  <div id="app">
    <portfolio></portfolio>
  </div>
</template>

<script>
import Portfolio from './components/Portfolio'

export default {
  name: 'app',
  components: {
    Portfolio
  }
}
</script>

<style>

#app {
  font-family: 'Roboto', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #424242;
  padding-top: 30px;
  text-align: center;
}
</style>
