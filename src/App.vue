<template>
  <CabecalhoGeral></CabecalhoGeral>
  <MainGeral></MainGeral>
  <FooterGeral></FooterGeral>
</template>

<script>
import CabecalhoGeral from './components/Head/CabecalhoGeral.vue';
import MainGeral from './components/Main/MainGeral.vue';
import FooterGeral from './components/Footer/FooterGeral.vue';


export default {
  name: 'App',
  components: {
    CabecalhoGeral,
    MainGeral,
    FooterGeral
}
}
</script>

<style>
  *{
    margin: 0;
    padding: 0;
    font-family: 'Inconsolata', monospace;
  }
</style>
