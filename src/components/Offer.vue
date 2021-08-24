<template>
  <section id="oferta">
    <div class="offer">
      <h4>Łączymy rzemiosło z pasją, tradycję z nowoczesnością</h4>
      <h2>LUCJAN`S BARBER SHOP<br />CUT-SHAVE-COFFE</h2>
      <p>Słowem – zadbamy kompleksowo o Twój wizerunek, włosy i zarost:</p>
      <div class="offer--list">
        <OfferItem
          v-for="link in links"
          :key="link.id"
          :name="link.name"
          :offer1="link.offer1"
          :offer2="link.offer2"
          :image="link.image"
        />
      </div>
    </div>
  </section>
</template>

<script>
import OfferItem from "./OfferItem.vue";
export default {
  name: "Offer",
  data() {
    return {
      links: [
        {
          id: 1,
          name: "CUTS",
          offer1: "Klasyczne strzyżenie (30 min.) 50 zł",
          offer2: "Królewskie strzyżenie (60 min.) 70 zł",
          image: "../assets/scissors.png",
        },
        {
          id: 2,
          name: "SHAVES",
          offer1: "Golenie klasyczne (30min) 40zł",
          offer2: "Królewskie golenie (30 min.) 70 zł",
          image: "../assets/razor.png",
        },
        {
          id: 3,
          name: "COMBOS",
          offer1: "Komplet (30 min.) 80 zł",
          offer2: "Tuszowanie siwizny (30 min.) 50-100 zł",
          image: "../assets/barber.png",
        },
      ],
    };
  },
  components: { OfferItem },
};
</script>

<style scoped>
section {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.offer {
  width: 80%;
  text-align: center;
  padding: 10rem 0rem;
}

.offer--list {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
}

h2 {
  font-size: 3rem;
  margin-top: 2rem;
}

h4 {
  font-style: italic;
}

h4::before {
  content: "";
  display: inline-block;
  width: 20px;
  height: 1px;
  border-bottom: 1px solid #000;
  margin: 0px 14px 4px;
}

h4::after {
  content: "";
  display: inline-block;
  width: 20px;
  height: 1px;
  border-bottom: 1px solid #000;
  margin: 0px 14px 4px;
}

p {
  margin-top: 2rem;
  color: #b59472;
}
</style>
