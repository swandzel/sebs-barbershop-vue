<template>
  <section id="kontakt">
    <div class="contact">
      <div class="contact--image">
        <img :src="image" />
      </div>
      <div class="contact--details">
        <h4>Seb's Barbershop</h4>
        <p>ul. Fryzjerska 3/1, Kraków</p>
        <p>500-000-789</p>
        <h5>Znajdź nas w mediach społecznościowy</h5>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Contact",
  data() {
    return {
      image: require("../assets/contact.jpg"),
    };
  },
};
</script>

<style scoped>
section {
  background: #000;
  color: #e7ecef;
}
.contact {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: center;
}

.contact--image {
  width: 700px;
  height: 500px;
}

img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
