<template>
  <div class="banner-container">

    <div class="container">
      <div class="texto-container">
      <img src="../assets/Folhas/port.png" alt="" />
      <img src="../assets/Folhas/fólio.png" alt="" />
    </div>
    <div class="folhas-container">
      <img src="../assets/Folhas/Folha1.png" alt="Logo" />
      <img src="../assets/Folhas/Folha3.png" alt="Logo" />
      <img src="../assets/Folhas/Folha1.png" alt="Logo" />
      <img src="../assets/Folhas/Folha2.png" alt="Logo" />
      <img src="../assets/Folhas/Folha5.png" alt="Logo" />
    </div>
    </div>
  </div>
</template>



<style scoped>
.banner-container {
  background-color: #fafafa;
  /* background: linear-gradient(122.83deg, #2a6751 20.19%, #448a43 99.92%); */
  height: 100vw !important;
}
.texto-container{
  display: flex;
  justify-content: center;
  margin-left: -20px;
}
.folhas-container {
  display: flex;
  justify-content: center;
}
.folhas-container img {
  position: absolute;
}
.texto-container {
  display: flex;
  justify-content: center;
}
.texto-container img:nth-child(1) {
  position: absolute;
  margin-right: 335px;
  z-index: 3;
}
.texto-container img:nth-child(2) {
  position: absolute;
  margin-top: 109px;
  margin-left: 335px;
  height: auto;
  z-index: 1;
}

.texto-container img {
  top: 180px;
}

/* Estilos para dispositivos de desktop */
@media only screen and (min-width: 1025px) {
  .banner-container {
    height: 650px !important;
  }
  .texto-container img {
    width: 380px;
  }
  .texto-container img:nth-child(1) {
    margin-right: 335px;
  }
  .texto-container img:nth-child(2) {
    margin-top: 19px;
    margin-left: 335px;
  }
  .folhas-container img {
    margin: 0 auto;
    position: absolute;
    width: 25%;
    height: auto;
  }

  .folhas-container img:nth-child(4) {
    top: -4%;
    right: 70%;

    z-index: 4;
    transform: rotate(-105deg);
  }
}
/* Estilos para tablets */
@media only screen and (min-width: 768px) and (max-width: 1024px) {
  .banner-container {
    background: linear-gradient(122.83deg, #2a6751 20.19%, #448a43 99.92%);
    height: 550px !important;
  }
  .texto-container img {
    width: 200px;
  }
  .texto-container img:nth-child(1) {
    margin-top: 52px;
    margin-right: 178px;
  }
  .texto-container img:nth-child(2) {
    margin-top: 109px;
    margin-left: 178px;
  }
  .folhas-container img {
    margin: 0 auto;
    position: absolute;
    width: 30%;
    height: auto;
  }
}

@media only screen and (max-width: 767px) {
  .banner-container {
    /* background-color: #75ad9d !important; */
    background: linear-gradient(122.83deg, #2a6751 20.19%, #448a43 99.92%);
    height: 450px !important;
  }
  .texto-container img {
    width: 140px;
  }
  .texto-container img:nth-child(1) {
    margin-top: 68px;
    margin-right: 120.15px;
  }
  .texto-container img:nth-child(2) {
    margin-left: 120.15px;
  }

  @keyframes moverGirar1 {
    0% {
      margin-top: 10px;
      margin-right: 12px;
      transform: rotate(200deg);
    }
    25% {
      margin-top: 120px;
      margin-right: 172px;
      transform: rotate(250deg);
    }
    100% {
      /* Mantém a posição final */
      margin-top: 120px;
      margin-right: 172px;
      transform: rotate(250deg);
    }
  }
  @keyframes moverGirar2 {
    0% {
      margin-top: 10px;
      margin-right: -200px;
      transform: rotate(60deg);
    }
    25% {
      margin-top: 10px;
      margin-right: -200px;
      transform: rotate(20deg);
    }
    100% {
      margin-top: 100px;
      margin-left: 180px;
      transform: rotate(230deg);
    }
  }
  @keyframes moverGirar3 {
    0% {
      margin-top: 20px;
      margin-right: -30px;
      transform: rotate(80deg);
    }
    25% {
      margin-top: 20px;
      margin-right: -40px;
      transform: rotate(80deg);
    }
    60% {
      transform: rotate(200deg);
    }
    100% {
      margin-top: 200px;
      margin-left: 240px;
      transform: rotate(80deg);
    }
  }
  @keyframes moverGirar4 {
    0% {
      margin-top: 26px;
      margin-left: -330px;
      transform: rotate(300deg);
    }
    5% {
      margin-top: 26px;
      margin-left: -330px;
      transform: rotate(300deg);
    }
    100% {
      margin-top: 260px;
      margin-left: 230px;
      transform: rotate(0deg);
    }
  }
  @keyframes moverGirar5 {
    0% {
      margin-top: 26px;
      margin-left: -330px;
      transform: rotate(300deg);
    }
    5% {
      margin-top: 26px;
      margin-left: -330px;
      transform: rotate(300deg);
    }
    100% {
      margin-top: 260px;
      margin-right: 75px;
      transform: rotate(135deg);
    }
  }

  .folhas-container {
    padding-top: 57px;

  }
  .folhas-container img {

    width: 120px;
  }

  .folhas-container img:nth-child(1) {
    z-index: 3;
    animation: moverGirar1 12s ease-in-out forwards;
  }

  .folhas-container img:nth-child(2) {
    z-index: 2;
    animation: moverGirar2 4s ease-in-out forwards;
  }

  .folhas-container img:nth-child(3) {
    z-index: 2;
    animation: moverGirar3 4s ease-in-out forwards;
  }
  .folhas-container img:nth-child(4) {
    z-index: 2;
    animation: moverGirar4 4s ease-in-out forwards;
  }
  .folhas-container img:nth-child(5) {
    z-index: 2;
    animation: moverGirar5 4s ease-in-out forwards;
  }
}
</style>

<script>
//import PortAsset from "../../assets/PortAsset.vue";
//import FolioAsset from "../../assets/FolioAsset.vue";

export default {
  name: "HomeComponent",
  components: {
    // ButtonQuadrado,
    //  PortAsset,
    //FolioAsset,
  },
};
</script>
