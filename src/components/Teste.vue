<template>
  <div>
    teste
    <button @click.prevent="chamar">teste</button>
  </div>
</template>

<script>

import Vue from 'vue'
import bus from '../utils/events/bus'

export default {
  name: 'teste',
  data () {
    return {
      msg: 'testee'
    }
  },
  created() {


  },
  methods:{
    chamar(){
      bus.$emit('foi-clicado', 13)
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
