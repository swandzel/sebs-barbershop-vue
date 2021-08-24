<template>
  <main>
    <About />
  </main>
</template>

<script>
import About from "./About.vue";
export default {
  name: "Main",
  components: { About },
};
</script>

<style scoped>
main {
  background: #e7ecef;
}
</style>
