<template>
  <section id="o-nas">
    <div class="about">
      <h4>Witaj w męskim świecie</h4>
      <h2>Trafiłeś w ręce fachowców</h2>

      <p>
        Z pasji do fryzjerstwa w 2014 roku powstał Lucjan`s Barber Shop,
        najbardziej męski salon w mieście. Pracujemy na najlepszych na rynku
        kosmetykach przeznaczonych właśnie dla mężczyzn.
      </p>
      <p>
        Wyróżnia nas pro aktywne nastawienie do klienta oraz nowatorskie
        podejście do sztuki jaką jest fryzjerstwo. Zamiłowanie do zawodu i chęć
        doskonalenia swoich umiejętności pozwoliły na stworzenie szerokiej gamy
        usług przeznaczonych dla najbardziej wymagających mężczyzn, począwszy od
        strzyżenia przez koloryzację, a skończywszy na kompletnej pielęgnacji
        włosów.
      </p>
      <p>
        Stworzyliśmy zespół fachowców którzy kochają swoją pracę. Świadczymy
        usługi na najwyższym poziomie… na takim , na jakim sami chcielibyśmy być
        obsługiwani.
      </p>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      name: "About",
    };
  },
};
</script>

<style scoped>
section {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.about {
  width: 80%;
  text-align: center;
  padding: 10rem 0rem;
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

h2 {
  font-size: 3rem;
}

p {
  margin-top: 2rem;
  color: #b59472;
}
</style>
