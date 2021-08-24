<template>
  <main>
    <About />
    <Book />
  </main>
</template>

<script>
import About from "./About.vue";
import Book from "./Book.vue";
export default {
  name: "Main",
  components: { About, Book },
};
</script>

<style scoped>
main {
  background: #e7ecef;
}
</style>
