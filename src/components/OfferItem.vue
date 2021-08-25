<template>
  <div class="offer--item">
    <img :src="image" />
    <!-- <h4>CUTS</h4>
    <p>Klasyczne strzyżenie (30 min.) 50 zł</p>
    <p>Królewskie strzyżenie (60 min.) 70</p> -->
    <h4>{{ name }}</h4>
    <p>{{ offer1 }}</p>
    <p>{{ offer2 }}</p>
    <Button
      :buttonText="buttonText"
      style="border: 2px solid #000; color: #000"
    />
  </div>
</template>

<script>
import Button from "./Button.vue";
export default {
  name: "OfferList",
  data() {
    return {
      buttonText: "Zarezerwuj termin",
    };
  },
  components: { Button },
  props: {
    id: Number,
    name: String,
    offer1: String,
    offer2: String,
    image: String,
  },
};
</script>

<style scoped>
.offer--item {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

img {
  width: 100px;
  height: auto;
  margin: 80px 0px 40px 0px;
}

h4 {
  font-weight: 200;
  margin-bottom: 1rem;
}

p {
  font-size: 1.25rem;
  font-weight: bold;
  margin-bottom: 1rem;
}
</style>
