<template>
  <main>
    <CardProduto v-for="dado in dados" :key="dado.nome"
    :url="dado.url" :nome="dado.nome" :descricao="dado.descricao"
    />
  </main>
</template>

<script>
import CardProduto from './CardProduto.vue';
import Dados from './Dados'

export default {
  name: 'MainGeral',
  components: { CardProduto },
  data(){
    return{
      dados: Dados
    }
  }  
}
</script>

<style>
  main{
    width: 100%;
    min-height: 30vh;
    padding-top: 20vh;
    padding-bottom: 20vh;

    display: grid;
    grid-template-columns: 23.34% 23.34% 23.34%;
    row-gap: 40px;
    justify-content: center;
    justify-items: center;
  }
</style>