<template>
  <div class="book">
    <div class="book--image">
      <img src="../assets/about-us.jpg" />
    </div>
    <div class="book--details">
      <h4>6 dni w tygodniu</h4>

      <h2>Czekamy na Ciebie</h2>

      <p>
        Nasze drzwi zawsze stoją przed Tobą otworem. Jeżeli chcesz dowiedzieć
        się czegoś więcej o naszych usługach lub po prostu porozmawiać - wpadaj
        w każdej chwili!
      </p>
      <p>
        Jeżeli jesteś już zdecydowany i chcesz zarezerwować sobie termin -
        skorzystaj z naszego internetowego systemu do rezerwacji i umów się na
        spotkanie z wybranym golibrodą.
      </p>
      <p>
        Działamy od poniedziałku do piątku w godzinach 8:00-21:00, a w soboty od
        8:00 do 14:00.
      </p>
      <Button :buttonText="buttonText" />
    </div>
  </div>
</template>

<script>
import Button from "./Button.vue";
export default {
  name: "Book",
  data() {
    return {
      buttonText: "Zarezerwuj termin",
    };
  },
  components: { Button },
};
</script>

<style scoped>
.book {
  display: flex;
  flex-direction: row;
  align-items: center;
  background: #000;
  font-size: 1.25rem;
  color: #e7ecef;
}

.book--image {
  width: 50%;
  /* height: 100vh; */
}

.book--image img {
  width: 100%;
  height: 100vh;
  object-fit: cover;
}

.book--details {
  padding: 0px 180px;
  width: 50%;
}

h4 {
  color: #b59472;
  letter-spacing: 2px;
}

h2 {
  font-size: 3rem;
}

p {
  margin-top: 2rem;
  font-weight: 300;
}
</style>
