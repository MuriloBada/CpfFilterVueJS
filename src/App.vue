<template>
  <div id="app">
    
    <CpfFilter :CPF="cpf" />
    
  </div>
</template>

<script>
import CpfFilter from './components/CpfFilter.vue'

export default {
  components:{
    CpfFilter
  },
  data(){
    return{
      cpf: '11360557970'
    }
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
