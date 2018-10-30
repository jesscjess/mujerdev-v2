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
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'

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
@import './assets/_variables.scss';

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.c-panel{
  display: flex;

  @include respond-above(md) {
    min-height: 650px;
    height: 100vh;
  }
}

.no-padding{
  padding: 0 !important;
}

.no-margin{
  margin: 0 !important;
}

@include respond-below(md) {

  .h-full-screen-height{
    height: 100vh;
    max-height: 620px;
  }
}


</style>
