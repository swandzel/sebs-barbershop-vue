<template>
  <header id="start">
    <div class="header--text">
      <h2>Cracow's Barber</h2>
      <h4>Since 2010</h4>
    </div>
    <Button :buttonText="buttonText" />
  </header>
</template>

<script>
import Button from "./Button.vue";
export default {
  data() {
    return {
      buttonText: "Zarezerwuj termin",
    };
  },
  name: "Header",
  components: { Button },
};
</script>

<style scoped>
header {
  display: flex;
  flex-direction: column;
  height: 100vh;
  width: 100%;
  justify-content: center;
  align-items: center;
  background-image: url("../assets/header.jpg");
  background-position: "center";
  background-size: "cover";
  background-repeat: "no-repeat";
}

.header--text {
  display: flex;
  flex-direction: column;
  color: #e7ecef;
  font-family: "Lora", serif;
  text-align: center;
  margin-top: 100px;
}
h2 {
  font-size: 6rem;
  text-transform: uppercase;
}
h4 {
  font-size: 2rem;
  letter-spacing: 6px;
}
</style>
