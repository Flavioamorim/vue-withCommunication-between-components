<template>
  <div class="hello">
    <h2>Ecosystem</h2>

  </div>
</template>

<script>

import Vue from 'vue'
import bus from '../utils/events/bus'

export default {
  name: 'hello',
  methods:{
        respondeu() {
            //this.frase = 'Daqui a pouco eu vou! Me traga uma cerveja.';
            console.log('respondendo....')
        },
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  mounted(){
    bus.$on('foi-clicado', () => console.log("aqui teste"))
  }
}
</script>

