<template>
  <div class="capa">
    <header>
      <h5>LOGO</h5>
      <h5>MENU</h5>
    </header>
      <div class="titulo">
        <span>TITULO</span>
      </div>
      <div class="texto">
        <span>
          Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.
        </span>
      </div>
  </div>
</template>

<script>

export default {
  name: 'CabecalhoGeral'
}
</script>

<style>
  .capa{
    width: 100%;
    height: 60vh;
    background-color: antiquewhite;

    display: grid;
    grid-template-columns: 35% 35%;
    grid-template-rows: 10vh 50vh;
    grid-template-areas: 'a a' 'b c';
    justify-content: center;
  }

  header{
    display: flex;
    align-items: center;
    justify-content: space-between;
    font-size: 30px;
    grid-area: a;
  }

  .titulo{
    grid-area: b;
    display: flex;
  }
  .titulo > span{
    font-size: 50px;
    margin-top: 18vh;
  }
  .texto{
    grid-area: c;
    display: flex;
  }
  .texto>span{
    font-size: 18px;
    margin-top: 18vh;
  }
</style>