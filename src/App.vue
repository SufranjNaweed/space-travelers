<template>
  <div id="app">
    <Hero />
  </div>
</template>

<script>
import Hero from './components/Hero'
export default {
  name: 'App',
  components: { Hero }
}
</script>

<style lang="scss">
*{
  box-sizing: border-box;
}
#app {
  font-family: 'Montserrat', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
