<template>
 <div id="cliente">
    <h2>Lista de produtos</h2>
    <Produto/>
 </div>

</template>

<script>
import Produto from './Produto';
export default {
  name: 'Cliente',
  components:{
    Produto
  }
}
</script>

<style>
    #cliente{
      color:blue;
      background:black;
      width: 100%;
      max-width: 300px;
      height: 300px;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
    }
  
</style>