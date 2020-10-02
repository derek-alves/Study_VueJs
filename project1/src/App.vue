<template>
  <div id="app">
    <h1>Cliente</h1>
    <Cliente :cliente="clientDerek" :showIdade="false"/>
    <Cliente :cliente="clientDerek" :showIdade="true"/>
    <Cliente :cliente="clientDerek" :showIdade="false"/>
    <Cliente :cliente="clientDerek" :showIdade="true"/>
    <Cliente :cliente="clientDerek" :showIdade="false"/>
    <!-- <Cliente nome="Timão" idade="330" showIdade="true"/> -->

  </div>
</template>

<script>
 import Cliente from './components/Cliente';

export default {
  name: 'App',

  data(){
    return{
        nomeDoDerek:'Derek E. Alves',
        clientDerek:{
          nome:"Derek",
          email:"derekão@derek.com",
          idade:28
        }
    }
  },

  components:{
    Cliente
  }
}
</script>

<style>
  #app{
    font-family: Arial, Helvetica, sans-serif;
    -webkit-font-smoothing:antialiased;
    -moz-osx-font-smoothing:grayscale;
    color:'#2c3e50';
    margin-top: 60px;
   
  }
</style>