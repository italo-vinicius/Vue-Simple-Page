<template>
  <header>
    <NavBar />
    <Picture />
  </header>
  <section>
    <main>
      <Users />
      <Main />
      <Main />
      <Main />
      <Main />
      <Form/>
    </main>
  </section>
  <footer>
    <Footer />
  </footer>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import Users from "./components/Users.vue";
import Picture from "./components/Picture.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";
import Form from "./components/Form.vue";
export default {
  name: "App",
  components: {
    NavBar,
    Main,
    Footer,
    Picture,
    Users,
    Form,
  },
};
</script>
