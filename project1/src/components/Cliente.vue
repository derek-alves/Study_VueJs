<template>
 <div id="cliente">
   <h4>Nome:{{cliente.nome}}</h4>
   <hr>
   <p>Email: {{cliente.email}}</p>
   <p v-if="showIdade">Idade:{{cliente.idade}}</p>
   <!-- <p v-show="showIdade">Idade:{{cliente.idade}}</p> -->
   <!-- <p v-else>Esse usuário escondeu a idade</p> -->
   <p v-else-if="cliente.idade > 20">Esse usuário não está vivo</p>
 </div>

</template>

<script>
// import Produto from './Produto';
export default {
  
  data(){
    return{
      descrição:'Programdor de camelo branco',
      numero:333333333,
      email:'derek@jupter.com'
    }
  },

  props:{
    cliente:Object,
    showIdade:Boolean
  }

  // name: 'Cliente',
  // components:{
  //   Produto
  // }
}
</script>

<style>
#cliente{
    background-color: rgb(201, 229, 253);
    width: 400px;
    padding: 2%;
    margin-top: 2%;
}
    
  
</style>