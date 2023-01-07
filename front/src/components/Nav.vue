<template>
  <header>
    <div class="logo">
      <img
        src="../assets/img/logo/Logo_apki.png"
        style="height: 100%; width: 100%; object-fit: contain"
      />
    </div>
    <div id="burger">Menu</div>
    <nav>
      <ol>
        <li @click="$emit('changePage', 0)">Strona Główna</li>
        <li @click="$emit('changePage', 1)">Produkty</li>
        <li @click="$emit('changePage', 2)">Zaloguj</li>
        <li @click="$emit('changePage', 3)">Zarejestruj</li>
      </ol>
    </nav>
  </header>
</template>

<style scoped>
header {
  padding: 5px 0px;
  background-color: #495f7a;
  height: 70px;
  font-family: "Nunito", sans-serif;
  display: flex;
  align-items: center;
  justify-content: space-between;
  font-weight: 600;
  color: #e1ecfa;
  position: relative;
}
.logo {
  height: 100%;
  width: 300px;
}
ol {
  display: flex;
  align-items: center;
  list-style: none;
  margin-right: 30px;
}
li {
  margin: 0px 10px;
  font-size: 1.3rem;
  transition: all 1s;
  cursor: pointer;
}
li:hover {
  font-size: 1.7rem;
}

#burger {
  display: none;
}

@media (max-width: 992px) {
  #burger {
    display: block;
    position: absolute;
    font-size: 1.3rem;
    top: 30%;
    right: 20px;
  }
  ol {
    display: none;
  }
}
</style>

<script>
export default {
  name: "Nav",
  methods: {
    baclToIndex() {
      console.log("baclToInde");
    },
  },
};
</script>
