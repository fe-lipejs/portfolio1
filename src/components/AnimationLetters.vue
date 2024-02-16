<template>
  <div>
    <br />
    <div class="container">
      <span>WHO AM I?</span>

      <img src="../../public/profile_photo.png" class="image" />
      <br /><br />
      <div class="name-container">
        <span>FELIPE S. JESUS</span>
        <span>DEV WEB JUNIOR</span>
      </div>
      <br /><br />
      <div style="text-align: justify">
        Olá, eu sou Felipe Santos, estudante de Sistemas de Informação na UVV e
        estou buscando oportunidades para ingressar na área de Design.
        <br /><br />
        Com uma paixão de longa data pela programação e pela criatividade, estou
        pronto para aplicar meus conhecimentos e contribuir para projetos
        inovadores.
        <!-- <br /><br />
        Estou aberto a estágios, freelas e colaborações que me permitam crescer
        profissionalmente e fazer a diferença no mundo do design. Vamos criar
        algo incrível juntos! -->
      </div>
      <br /><br /><br><br>
      <div class="button">SEND A PROPOSAL</div>
    </div>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  flex-direction: column;
  padding-inline: 60px;
}
.container span {
  font-family: "Poppins", sans-serif;
  font-weight: bolder;
  font-size: 40px;
  line-height: 120px;
  color: #000000;
}

.container img {
  height: auto;
  width: 50%;
  margin: 0 auto;
}
.name-container {
  display: flex;
  justify-content: center;
  flex-direction: column;
  font-family: "Roboto", sans-serif;
  color: #000000;
}
.name-container span {
  font-weight: normal;
  font-size: 20px;
  line-height: 28px;
}

.name-container span:nth-child(1) {
  color: #5ec666;
  font-weight: bolder;
  font-size: 28px;
}
.button {
  margin: 0 auto;
  padding: 20px 30%;
  background: #2d2a28;
  border-radius: 100px;
  color: #fff;
  font-weight: bold;
}
</style>