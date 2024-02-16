<template>
  <div>
    <BannerComponent/>
    <AnimationLetters/>

  </div>
</template>

<style scoped>
.banner-container {
  display: flex;
  flex-direction: column;
  /* justify-content: space-around; */
  width: 100%;
  height: 580px;
  background-color: #fafafa;
}

.banner-container div {
  width: 60%;
}
.banner-container div:nth-child(2) {
  /* display: flex; */
  flex-direction: column;
  justify-content: space-around;
  width: 40%;
}
.folhas-container div {
  margin: 0 auto;
  /* background-color: red; */
}
.texto-container {
  background-color: rgb(41, 41, 41);
  padding: 100px;
  color: #eeeeee;
}
.texto-container div {
  width: 100%;
}
</style>

<script>
//import ButtonQuadrado from "../components/ButtonQuadrado.vue";
import BannerComponent from "../components/BannerComponent.vue";
import AnimationLetters from "../components/AnimationLetters.vue";

export default {
  name: "HomeComponent",
  components: {
   // ButtonQuadrado,
    BannerComponent,
    AnimationLetters,
  },
};
</script>