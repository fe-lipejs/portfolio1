<template>
  <div>
    <MenuComponent />
    <HomeComponent />
  </div>
</template>

<script>
import HomeComponent from "./components/HomeComponent.vue";
import MenuComponent from "./components/MenuComponent.vue";

export default {
  name: "App",
  components: {
    HomeComponent,
    MenuComponent,
  },
};
</script>

<style>
@import "~typeface-roboto";
* {
  padding: 0;
  margin: 0;
}
#app {
  font-family: 'Roboto', sans-serif !important;
  text-align: center;

}
</style>
