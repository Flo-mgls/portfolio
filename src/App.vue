<template>
  <header>
    <NavBar />
    <Header />
  </header>
  <Intro />
</template>

<script>
import NavBar from "./components/NavBar.vue";
import Header from "./components/Header.vue";
import Intro from "./components/Intro.vue";

export default {
  name: "App",
  components: {
    NavBar,
    Header,
    Intro,
  },
};
</script>

<style lang="scss">
#app {
  font-family: "Quicksand", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #455A64;
}
</style>
