<template>
  <main>
    <About />
    <Book />
    <Offer />
    <Team />
    <Training />
    <Contact />
  </main>
</template>

<script>
import About from "./About.vue";
import Book from "./Book.vue";
import Offer from "./Offer.vue";
import Team from "./Team.vue";
import Training from "./Training.vue";
import Contact from "./Contact.vue";
export default {
  name: "Main",
  components: { About, Book, Offer, Team, Training, Contact },
};
</script>

<style scoped>
main {
  background: #e7ecef;
}
</style>
