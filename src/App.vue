<template>
  <div id="app">
    <AppHeader />
    <AppMain />
    <TravelCard />
  </div>
</template>

<script>
import AppMain from "./components/app/app-main.vue";
import AppHeader from "./components/app/app-header.vue";
import TravelCard from "./modules/travels/travel-card.vue";

export default {
  name: "App",
  components: {
    AppMain,
    AppHeader,
    TravelCard,
  },
};
</script>

<style>
* {
  box-sizing: border-box;
}
body {
  margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
