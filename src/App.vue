<template>
  <header><NavBar /></header>
  <section>
    <main>
      <Main />
      <Main />
      <Main />
      <Main />
      <Main />
      <Main />
    </main>
  </section>
  <footer>
      <Footer/>
  </footer>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue"
export default {
  name: "App",
  components: {
    NavBar,
    Main,
    Footer
  },
};
</script>
