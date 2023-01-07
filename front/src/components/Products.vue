<template>
  <div class="products">
    <div class="page">
      <div class="square">
        <div class="square__content">
          <h1 class="square__content--title">WhereIsMofMof3000</h1>
          <p>
            Twój pies znika na całe noce, a rano nie chce powiedzieć, które
            hydranty oznaczył? Dzięki WhereIsMofMof3000 nie musisz się już go
            pytać! Wystarczy, że podłączysz GPS-a, którego przez całą noc nosił
            pies i zalogujesz się do naszej aplikacji.
          </p>
          <a class="square__content--link" href="#"> Zamów już teraz!</a>
        </div>
        
        <div class="box__img">
          <img
            class="square__img"
            src="https://cinkciarz.pl/images/currency-exchange/currency-tools/services-top-img.png"
          />
        </div>
      </div>

      <div class="square">
        <div class="square__content">
          <h1 class="square__content--title">WhereIsŁofŁof3001</h1>
          <p class="square__content--content">
            Rozszerzona wersja WhereIsMofMof3000, dzięki której w czasie
            rzeczywistym jesteś w stanie sprawdzić, pod którym domem sąsiadów
            twój najukochańszy pupilek wyje serenady.
          </p>
          <a class="square__content--link" href="#"> Już wkrótce! </a>
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
