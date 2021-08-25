<template>
  <section id="kontakt">
    <div class="contact">
      <div class="contact--image">
        <img :src="image" />
      </div>
      <div class="contact--details">
        <h1>Seb's Barbershop</h1>
        <p>ul. Fryzjerska 3/1, Kraków</p>
        <p>500-000-789</p>
        <h5>Znajdź nas w mediach społecznościowy</h5>
        <div class="social-media">
          <i class="fab fa-facebook fa-3x"></i>
          <i class="fab fa-instagram fa-3x"></i>
          <i class="fab fa-pinterest fa-3x"></i>
        </div>
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
  flex: 1;
}
.contact--details {
  flex: 1;
  text-align: center;
}

img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

h1 {
  font-size: 2.5rem;
  font-family: "Gloria Hallelujah", cursive;
}

h5 {
  padding-top: 1rem;
}

.social-media {
  display: flex;
  flex-direction: row;
  justify-content: center;
}

i {
  margin: 20px;
  cursor: pointer;
}
</style>
