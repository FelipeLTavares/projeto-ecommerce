<template>
  <header>
    <nav> HELLO WORLD</nav>
    <img src="https://i.picsum.photos/id/1/5616/3744.jpg?hmac=kKHwwU8s46oNettHKwJ24qOlIAsWN9d2TtsXDoCWWsQ" alt="Imagem Header">
  </header>
</template>

<script>
export default {
  name: 'CabecalhoGeral'
}
</script>

<style>
  header{
    border: 1px solid red;
    width: 100%;
    height: 100vh;
    background-color: black;
    overflow: hidden;
  }
  header>nav{
    width: 100%;
    height: 80px;
    background-color: rgb(255, 228, 196, 0.1);
    position: absolute;
  }
  header>img{
    object-fit: cover;
    width: 100%;
    height: 100vh;
  }
</style>