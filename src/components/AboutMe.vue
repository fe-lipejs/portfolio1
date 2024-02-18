<template>
  <div class="aboutme-container" ref="aboutmeContainer" @mousemove="moveCircleWithMouse" @touchmove="moveCircleWithTouch">
    <div class="circle" ref="circle"></div>

    <div class="container">
      <span>WHO AM I?</span>

      <img src="../../public/profile_photo.png" class="image" />
      <br /><br />
      <div class="name-container">
        <span>FELIPE S. JESUS</span>
        <span>DEV WEB JUNIOR</span>
      </div>
      <br /><br />
      <div style="text-align: justify; color: #f5f5f5; font-weight: lighter">
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
      <br /><br /><br /><br />
      <div class="button">CONTACT</div>
      <br /><br /><br /><br />
    </div>
  </div>
</template>

<style scoped>

.aboutme-container {
  display: none;
  display: flex;
  justify-content: center !important;
  flex-direction: column;
  width: 100%;
  background-color: #090909;
  /* background-color: red; */
}
.circle {
  position: absolute;
  border-radius: 100%;
  width: 500px;
  height: 500px;
  border: 3px solid #5ec6671b;
  z-index: 8;
}
.container {
  /* position: absolute; */
  display: flex;
  justify-content: center;
  flex-direction: column;
  padding-inline: 30px;
  max-width: 500px;
  margin: 0 auto;
  z-index: 10;
}
.container span {
  font-family: "Poppins", sans-serif;
  font-weight: bolder;
  font-size: 40px;
  line-height: 120px;
  color: #5ec666;
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
  color: #ffff;
}
.name-container span {
  font-weight: bold;
  font-size: 20px;
  line-height: 28px;
}

.name-container span:nth-child(1) {
  color: #5ec666;
  font-weight: bolder;
  font-size: 20px;
}
.name-container span:nth-child(2) {
  color: #eee;
  font-weight: normal;
  font-size: 14px;
  line-height: 12px;
}
.button {
  /* margin: 0 auto; */
  display: grid;
  justify-items: center !important;
  align-items: center;
  height: 40px;
  width: 100%;
  background: #5ec666;
  /* background: #fff; */
  border-radius: 100px;
  color: #000;
  font-size: 14px;
  font-weight: bolder;
}
</style>


<script>
export default {
  mounted() {
    this.startMovingCircle();
  },
  methods: {
    startMovingCircle() {
      // Chama a função moveCircle a cada 2 segundos
      this.moveCircle(); // Chamada inicial
      setInterval(this.moveCircle, 3000);
    },
    moveCircle() {
      const aboutmeContainer = this.$refs.aboutmeContainer;
      const circle = this.$refs.circle;

      const containerWidth = aboutmeContainer.offsetWidth;
      const containerHeight = aboutmeContainer.offsetHeight;
      const circleSize = circle.offsetWidth;

      const randomX = Math.random() * (containerWidth - circleSize);
      const randomY = Math.random() * (containerHeight - circleSize);

      circle.style.left = `${randomX}px`;
      circle.style.top = `${randomY}px`;

      // Animação para suavizar o movimento
      circle.style.transition = 'left 2s ease-in-out, top 2s ease-in-out';
    }
  }
}
</script>





