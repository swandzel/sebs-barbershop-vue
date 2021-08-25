<template>
  <Navbar />
  <Header />
  <Main />
  <Footer />
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";
export default {
  components: { Navbar, Header, Main, Footer },
  // methods: {
  //   scroll: new SmoothScroll('a[href*="#"]', {
  //     speed: 1000,
  //   }),
  // },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Lato:wght@300;400&family=Lora:wght@500&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Gloria+Hallelujah&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: "Lato", sans-serif;
  background: #37392e;
  /* font-family: "Lora", serif; */
}
</style>
