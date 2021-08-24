<template>
  <main>
    <About />
    <Book />
    <Offer />
  </main>
</template>

<script>
import About from "./About.vue";
import Book from "./Book.vue";
import Offer from "./Offer.vue";
export default {
  name: "Main",
  components: { About, Book, Offer },
};
</script>

<style scoped>
main {
  background: #e7ecef;
}
</style>
