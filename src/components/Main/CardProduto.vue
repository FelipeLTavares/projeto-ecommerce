<template>
  <div class="CardProduto">
    <img :src="url" :alt="nome">
    <span class="TituloProduto">{{nome}}</span>
    <span class="DescricaoProduto">{{descricao}}</span>
  </div>
</template>

<script>
export default {
  name: 'CardProduto',
  props:{
    url: String,
    nome: String,
    descricao: String
  }
}
</script>

<style>
  .CardProduto{
    width: 270px;
    height: 240px;
    overflow: hidden;
  }
  .CardProduto>img{
    width: 100%;
    height: 180px;
    transition: opacity 0.5s;
  }
  .CardProduto>img:hover{
    opacity: 0.8;
  }
  .CardProduto>span{
    display: flex;
    flex-direction: column;
  }
  .TituloProduto{
    font-size: 20px;
    font-weight: 600;
  }
  .DescricaoProduto{
    font-size: 14px;
  }
</style>