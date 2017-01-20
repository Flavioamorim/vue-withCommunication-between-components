<template>
  <div id="app">
    <img src="./assets/logo.png">
    <hello></hello>
    <teste></teste>
  </div>
</template>

<script>

import Hello from './components/Hello'
import Teste from './components/Teste'

import Vue from 'vue'
import bus from './utils/events/bus'

export default {
  name: 'app',
  components: {
    Hello,
    Teste
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
