<template>
  <footer>
    <div class="Sociais">
      <span>Instagram</span>
      <span>Facebook</span>
      <span>Twitter</span>
      <span>Whatsapp</span>
    </div>
    <div class="Opcoes">
      <span>Institucional</span>
      <span>Clientes</span>
      <span>Investidores</span>
      <span>Reclame Aqui</span>
    </div>
    <span class="DireitosReservados">Todos os Direitos Reservados</span>
  </footer>
</template>

<script>
export default {
  name: 'FooterGeral'
}
</script>

<style>
  footer{
    width: 100%;
    height: 40vh;
    background-color: #202020;
    color: white;

    display: grid;
    grid-template-columns: 35% 35%;
    grid-template-rows: 35vh 5vh;
    grid-template-areas: 'x y' 'z z';
    justify-content: center;
  }
  .Sociais,.Opcoes,.DireitosReservados{
    display: grid;
    grid-template-columns: auto;
  }
  .Sociais,.Opcoes{
    padding-top: 20px;
    align-content: flex-start;
  }
  .Sociais>span,.Opcoes>span{
    margin: 10px;
  }
  .Sociais>span:hover,.Opcoes>span:hover{
    color: orange;
    cursor: pointer;
  }
  .DireitosReservados{
    width: 100%;
    justify-content: center;
  }
  .Sociais{ grid-area: x;}
  .Opcoes{ grid-area: y;}
  .DireitosReservados{ grid-area: z;}

  @media(max-width: 1200px){
    .titulo > span{
      font-size: 44px;
    }
    .texto>span{
      font-size: 16px;
    }
  }

  @media(max-width:800px){
    footer{
      height: 66vh;
      display: grid;
      grid-template-columns: 70%;
      grid-template-rows: 30vh 30vh 6vh;
      grid-template-areas: 'x' 'y' 'z';
      justify-content: center;
    }
  }
</style>