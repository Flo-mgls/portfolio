<template>
  <header>
    <NavBar />
    <Header />
  </header>
  <main>
    <Intro />
    <Offers />
    <Skills />
    <Portfolio />
  </main>
  <footer>
    <Contact />
    <Footer />
  </footer>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import Header from "./components/Header.vue";
import Intro from "./components/Intro.vue";
import Offers from "./components/Offers.vue";
import Skills from "./components/Skills.vue";
import Portfolio from "./components/Portfolio.vue";
import Contact from "./components/Contact.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    NavBar,
    Header,
    Intro,
    Offers,
    Skills,
    Portfolio,
    Contact,
    Footer
  },
};
</script>

<style lang="scss">
#app {
  font-family: "Quicksand", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #455a64;
}
</style>
