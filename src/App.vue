<template>
  <img alt="Vue logo" style="width: 100px;" src="./assets/sunder-muthukumaran-fd6K_OFlnRA-unsplash.jpg">
  <GComponent />
</template>

<script>
import GComponent from './components/GComponent.vue'

export default {
  name: 'App',
  components: {

    GComponent
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
