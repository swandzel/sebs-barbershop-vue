<template>
  <section id="szkolenia">
    <div class="training">
      <h4>Indywidualne szkolenie 6 dniowe - 6000 zł</h4>
      <p>
        Nasze szkolenia 6-dniowe nastawione są na prawdziwą intensywną naukę
        rzemiosła fryzjera męskiego. Szkolenie ma charakter indywidualny, gdzie
        nasz edukator pracuje tylko z osobą szkoloną. Kładziemy nacisk na
        maksymalną ilość praktyki i szkolenie w konwencji look&work. Dzięki
        temu, uczestnicy naszych kursów, mogą z powodzeniem rozpocząć pracę w
        rzemiośle. W czasie szkoleń omawiamy pełny proces strzyżeń, golenia
        klasycznego, trymowania zarostu, technik fade, oraz omawiamy techniki
        obsługi klienta i odsprzedaży produktów.
      </p>
      <h2>Kto prowadzi szkolenia?</h2>
      <p>
        Autorami i prowadzącymi szkolenia są najbardziej doświadczeni barberzy z
        naszego salonu, którzy doskonalą swoje rzemiosło już od kilkunastu lat.
        Naszą siłą jest praktyka - najlepsze źródło wiedzy. Szkolenie przewiduje
        pracę z modelem, zgodnie z autorskim scenariuszem opracowanym w ramach
        ``Lucjan's Barber Shop Academy Look&Wok``. Wysoką efektywność szkolenia
        gwarantuje system pracy, gdzie część zadań wykonuje nauczyciel, a część
        uczeń pod stałym nadzorem opiekuna. Podczas całego szkolenia
        wykorzystujemy wyłącznie najwyższej jakości, niezawodny sprzęt i
        najlepsze kosmetyki. Nie stosujemy półśrodków. Zawsze stawiamy na to, co
        najlepsze.
      </p>

      <h2>Co osiągniesz dzięki szkoleniu?</h2>
      <ul>
        <li>Podniesiesz kwalifikacje zawodowe.</li>
        <li>Udoskonalisz warsztat barberski.</li>
        <li>Przekonasz się, jak wygląda praca na najlepszych kosmetykach.</li>
        <li>Wypracujesz najwyższe standardy obsługi klienta.</li>
        <li>Dowiesz się, jak zwiększyć odsprzedaż kosmetyków.</li>
        <li>Zdobędziesz certyfikat odpowiedniego stopnia.</li>
        <li>
          Przekonasz się, jak to jest pracować z ludźmi, którzy podchodzą do
          swojej pracy z pasją i pełnym zaangażowaniem.
        </li>
      </ul>

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

<style></style>
