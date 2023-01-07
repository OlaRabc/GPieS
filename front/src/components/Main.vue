<template>
  <div class="products">
    <div class="page">
      <div class="square">
        <div class="square__content">
          <h1 class="square__content--title">O nas</h1>
          <p class="square__content--content">
            Firma GPieS to przedsiębiorstwo, które specjalizuje się w produkcji
            oraz dystrybucji takich obroży. Obroże z GPS są przeznaczone dla
            właścicieli psów, którzy chcą mieć możliwość śledzenia położenia
            swojego psa w czasie rzeczywistym lub odtworzenia trasy, po której
            pies się poruszał. Obroże tego typu są często wyposażone w moduł GPS
            oraz łączność bezprzewodową, dzięki czemu właściciel może śledzić
            swojego psa za pomocą naszej strony internetowej.
          </p>
        </div>
        <div class="box__img border">
          <img
            class="square__img"
            src="https://cdn.benchmark.pl/uploads/backend_img/c/recenzje/2020_09/5411-darmowa-nawigacja-android/darmowa-nawigacja-gps.jpg"
          />
        </div>
      </div>

      <div class="square" >
        <div class="square__content">
          <h1 class="square__content--title">Technologie</h1>
          <p class="square__content--content">
            GPS wykorzystuje technologię satelitarną oraz technologię
            odbiorników sygnałów satelitarnych, aby umożliwić użytkownikom
            określenie ich położenia na Ziemi. Satelity GPS krążą wokół Ziemi na
            wysokości ponad 20 000 km i emitują sygnały radiowe, które są
            odbierane przez odbiorniki GPS znajdujące się na Ziemi. Każdy
            satelit emituje sygnał z unikalnym kodem, który jest odczytywany
            przez odbiornik. Odbiornik GPS oblicza swoje położenie, mierząc
            czas, jaki upłynął od wysłania sygnału przez satelitę do momentu
            odebrania go przez odbiornik. Im więcej satelitów odbierze sygnał,
            tym dokładniejszy będzie wynik.
          </p>
        </div>
        <div class="box__img border">
          <img
            class="square__img"
            src="https://a.allegroimg.com/s512/11b164/f2c0ae5f4df0a6b7bc7b810a8e1d/NANO-GPS-LOKALIZATOR-PODSLUCH-NAGRYWANIE-APLIKACJA"
          />
        </div>
      </div>

      <div class="square" id="currencyTools">
        <div class="square__content">
          <h1 class="square__content--title">Jak działa GPS</h1>
          <p class="square__content--content">
            GPS, czyli Global Positioning System, to system nawigacji
            satelitarnej opracowany przez amerykański rząd, który pozwala
            użytkownikom na określenie ich położenia na Ziemi z dużą
            dokładnością. Składa się z sieci satelitów, które krążą wokół Ziemi
            na wysokości ponad 20 000 km, oraz z odbiorników GPS, które są
            umieszczane w urządzeniach takich jak smartfony, nawigacje
            samochodowe i zegarki sportowe.
          </p>
        </div>
        <div class="box__img">
          <img
            class="square__img"
            src="https://cinkciarz.pl/images/currency-exchange/currency-tools/services-top-img.png"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.page {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  font-family: "Nunito", sans-serif;
  width: 100%;
  margin: 0 auto;
  overflow: hidden;
}

.box__img {
  max-width: 100%;
  min-width: 500px;
  margin-bottom: 32px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
}

@media (min-width: 1000px) {
  .box__img {
    max-width: 50%;
  }
}
.square {
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-direction: row;
  flex-wrap: wrap;
  padding-top: 100px;
}
.square__content {
  max-width: 35%;
  min-width: 500px;
  margin-bottom: 32px;
}
.square__content--link {
  text-decoration: none;
  color: #0b49db;
}
.square__content--content {
  margin-bottom: 32px;
}
.square__img {
  max-width: 100%;
  height: auto;
}

@media (min-width: 1000px) {
  .square:nth-child(2n) {
    flex-direction: row-reverse;
  }
}
.page {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  font-family: "Nunito", sans-serif;
  width: 100%;
  margin: 0 auto;
  overflow: hidden;
}

.box__img {
  max-width: 100%;
  min-width: 500px;
  margin-bottom: 32px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
}

@media (min-width: 1000px) {
  .box__img {
    max-width: 50%;
  }
}
.square {
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-direction: row;
  flex-wrap: wrap;
  padding-top: 100px;
}
.square__content {
  max-width: 35%;
  min-width: 500px;
  margin-bottom: 32px;
}
.square__content--link {
  text-decoration: none;
  color: #0b49db;
}
.square__content--content {
  margin-bottom: 32px;
}
.square__img {
  max-width: 100%;
  height: auto;
}

@media (min-width: 1000px) {
  .square:nth-child(2n) {
    flex-direction: row-reverse;
  }
}

.border{
  border-radius: 15px;
}
</style>

<script>
export default {
  name: "Soon",
  methods: {
    baclToIndex() {
      console.log("baclToInde");
    },
  },
};
</script>
