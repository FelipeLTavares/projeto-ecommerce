<template>
  <header>
    <nav>
      <span class="logo">LOGO</span>
      <div class="menu">
        <span>HOME</span>
        <span>HOME</span>
        <span>HOME</span>
        <MenuIcon class="menuIcon"></MenuIcon>
      </div>
    </nav>
    <img src="https://i.picsum.photos/id/6/5616/3744.jpg?hmac=OfsNapDl2Ndsw_54oKgnNRNYAMLv8mLZuHgEJUZ3O_I" alt="Imagem Header">
  </header>
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
  header{
    width: 100%;
    height: 100vh;
    background-color: black;
    overflow: hidden;
  }
  header>nav{
    width: 100%;
    height: 80px;
    background-color: rgb(7, 4, 0, 0.6);
    position: absolute;

    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  header>nav>.logo{
    margin: 20px;
    color: white;
    font-size: 45px;
    font-weight: 700;
  }
  header>nav>.menu{
    display: flex;

  }
  header>nav>.menu>span{
    color: white;
    font-size: 20px;
    font-weight: 600;
    padding: 26px;
  }
  header>nav>.menu>.menuIcon{
    display: none;
  }


  header>img{
    width: 100%;
    height: 100vh;
    object-fit: cover;
  }
</style>