<template>
  <div id="app">
    <HomePage />
  </div>
</template>

<script>
import HomePage from "./pages/home-page.vue";

export default {
  name: "App",
  components: {
    HomePage,
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
