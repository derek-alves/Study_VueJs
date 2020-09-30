<template>
 <div id="cliente">
   <h4>Nome:{{cliente.nome}}</h4>
   <hr>
   <p>Email: {{cliente.email}}</p>
   <p>Idade:{{cliente.idade}}</p>
  
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
    nome:String,
    idade:Number,
    cliente:Object
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