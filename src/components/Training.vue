<template>
  <section id="szkolenia">
    <div class="training">
      <h4>Chcesz zostać golibrodą?</h4>
      <h2>Indywidualne szkolenie 6 dniowe - 6000 zł</h2>
      <div class="training--about">
        Nasze szkolenia 6-dniowe nastawione są na prawdziwą intensywną naukę
        rzemiosła fryzjera męskiego. Szkolenie ma charakter indywidualny, gdzie
        nasz edukator pracuje tylko z osobą szkoloną. Kładziemy nacisk na
        maksymalną ilość praktyki i szkolenie w konwencji look&work. Dzięki
        temu, uczestnicy naszych kursów, mogą z powodzeniem rozpocząć pracę w
        rzemiośle. W czasie szkoleń omawiamy pełny proces strzyżeń, golenia
        klasycznego, trymowania zarostu, technik fade, oraz omawiamy techniki
        obsługi klienta i odsprzedaży produktów.
      </div>
      <div class="training--about-more">
        <div class="about--part">
          <h2>Kto prowadzi szkolenia?</h2>
          <p>
            Autorami i prowadzącymi szkolenia są najbardziej doświadczeni
            barberzy z naszego salonu, którzy doskonalą swoje rzemiosło już od
            kilkunastu lat. Naszą siłą jest praktyka - najlepsze źródło wiedzy.
            Szkolenie przewiduje pracę z modelem, zgodnie z autorskim
            scenariuszem opracowanym w ramach Seb's Barber Shop Academy
            Look & Work. Wysoką efektywność szkolenia gwarantuje system pracy,
            gdzie część zadań wykonuje nauczyciel, a część uczeń pod stałym
            nadzorem opiekuna. Podczas całego szkolenia wykorzystujemy wyłącznie
            najwyższej jakości, niezawodny sprzęt i najlepsze kosmetyki. Nie
            stosujemy półśrodków. Zawsze stawiamy na to, co najlepsze.
          </p>
        </div>
        <div class="about--part left">
          <h2>Co osiągniesz dzięki szkoleniu?</h2>
          <ul>
            <li>Podniesiesz kwalifikacje zawodowe.</li>
            <li>Udoskonalisz warsztat barberski.</li>
            <li>
              Przekonasz się, jak wygląda praca na najlepszych kosmetykach.
            </li>
            <li>Wypracujesz najwyższe standardy obsługi klienta.</li>
            <li>Dowiesz się, jak zwiększyć odsprzedaż kosmetyków.</li>
            <li>Zdobędziesz certyfikat odpowiedniego stopnia.</li>
            <li>
              Przekonasz się, jak to jest pracować z ludźmi, którzy podchodzą do
              swojej pracy z pasją i pełnym zaangażowaniem.
            </li>
          </ul>
        </div>
      </div>

      <Button
        :buttonText="buttonText"
        style="border: 2px solid #000; color: #000"
      />
    </div>
  </section>
</template>

<script>
import Button from "./Button.vue";
export default {
  name: "Training",
  data() {
    return {
      buttonText: "Zarezerwuj szkolenie",
    };
  },
  components: { Button },
};
</script>

<style scoped>
section {
  display: flex;
  justify-content: center;
  padding: 8rem 0rem;
}

.training {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 60%;
  text-align: center;
}
.training--about {
  color: #e7ecef;
  background: #000;
  padding: 20px 40px;
}

.training--about-more {
  display: flex;
  flex-direction: row;
  padding-top: 20px;
}

.about--part {
  flex: 1;
  padding: 20px 20px;
}

.left {
  text-align: left;
}

h2 {
  padding: 10px 0px;
}

h4 {
  font-style: italic;
  color: #000;
}

h4::before {
  content: "";
  display: inline-block;
  width: 20px;
  height: 1px;
  border-bottom: 1px solid #b59472;
  margin: 0px 14px 4px;
}

h4::after {
  content: "";
  display: inline-block;
  width: 20px;
  height: 1px;
  border-bottom: 1px solid #b59472;
  margin: 0px 14px 4px;
}
</style>
