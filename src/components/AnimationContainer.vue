<template>
  <div>
    <div class="container">
      <div :class="{ quadrado: animar }"></div>
    </div>
  </div>
</template>
<style scoped>
.container {
  display: flex;
  justify-content: center;
  background-color: rgb(255, 255, 255);
  padding-top: 40px;
  width: 100%;
  height: 300px;
}
.quadrado {
  position: absolute;
  /* margin: 0 auto; */
  background-color: lightgreen;
  width: 300px;
  height: 300px;
  animation: quadrado 1s ease-in-out forwards;
}
.quadrado {
  position: absolute;
  /* margin: 0 auto; */
  background-color: lightgreen;
  width: 300px;
  height: 300px;
  animation: quadrado1 1s ease-in-out forwards;
}
</style>

<script>
export default {
  data() {
    return {
      animar: false,
    };
  },
  mounted() {
    this.iniciarAnimacao();
  },
  methods: {
    iniciarAnimacao() {
      const style = document.createElement("style");
      const keyframe = [
        ` @keyframes quadrado {
                0% {
                    width: 200px;
                    height: 0px;
                    opacity: 0;
                }
                30% {
                    width: 200px;
                    height: 100px;
                    opacity: 0.5;
                }
                100% {
                    width: 200px;
                    height: 200px;
                    opacity: 1;
                }
            }`,
        ` @keyframes quadrado1 {
                0% {
                    width: 0px;
                    height: 2000px;
                    opacity: 0;
                }
                100% {
                    width: 200px;
                    height: 200px;
                    opacity: 1;
                }
            }`,
      ];

      for (let i = 0; i < 2; i++) {
        style.textContent = keyframe[i]
        document.head.appendChild(style);

        this.animar = true;
        setTimeout(() => {
          this.animar = false;
          console.log(i)
        }, 2000); // Tempo de duração da animação em milissegundos
      }
    },
  },
};
</script>
