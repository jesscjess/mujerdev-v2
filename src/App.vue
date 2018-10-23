<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <Welcome></Welcome>
    <MujerDev></MujerDev>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Welcome from './components/Welcome.vue'
import MujerDev from './components/MujerDev.vue'

export default {
  name: 'app',
  components: {
    HelloWorld,
    Welcome,
    MujerDev
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.c-panel{
  height: 100vh;
  min-height: 650px;
  display: flex;
}

.no-padding{
  padding: 0 !important;
}

</style>
