<template>
  <div class="capa">
    <header>
      <h5>LOGOTIPO</h5>
      <div class="menu">
        <span class="itemMenu">INICIO</span>
        <span class="itemMenu">PRODUTOS</span>
        <span class="itemMenu">CONTATO</span>
        <MenuIcon class="menuIc"></MenuIcon>
      </div>
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
import MenuIcon from 'vue-material-design-icons/Menu.vue';

export default {
  name: 'CabecalhoGeral',
  components:{
    MenuIcon
  }
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

  .menu{
    display: flex;
    align-items: center;
  }
  .menu>.itemMenu{
    font-size: 20px;
    padding: 10px;
  }
  .menu>.itemMenu:hover{
    font-weight: 700;
    font-size: 24px;
  }

  .menuIc{
    display: none;
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
    text-align: justify;
  }
  .texto>span{
    font-size: 18px;
    margin-top: 18vh;
  }

  @media(max-width: 1200px){
    .titulo > span{
      font-size: 44px;
    }
    .texto>span{
      font-size: 16px;
    }
  }

  @media(max-width:800px){
    .capa{
      grid-template-areas: 'a a' 'b b';
    }
    .menu>.itemMenu{
      display: none;
    }
    .menuIc{
      display: inline;
    }
    .titulo{
      justify-content: center;
    }
    .titulo > span{
      font-size: 40px;
    }
    .texto{
      display:none;
    }
  }
</style>