<template>
  <header>
    <div class="logo">
      <img
        src="../assets/img/logo/Logo_apki.png"
        style="height: 100%; width: 100%; object-fit: contain"
      />
    </div>
    <div id="burger">
      <div :class="[isMenuOpen?'close':'', 'menu__btn']" @click="isMenuOpen=!isMenuOpen">
        <div class="bar"></div>
        <div class="bar"></div>
        <div class="bar"></div>
      </div>
    </div>
    <nav :class="[isMenuOpen?'close':'', 'nav']">
      <ol>
        <li @click="$emit('changePage', 0)">Wyloguj</li>
      </ol>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Nav",
  data() {
    return {
      isMenuOpen: false
    }
  },
  methods: {
    baclToIndex() {
      console.log("baclToInde");
    },
  },
};
</script>

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

.menu__btn {
  top: 20px;
  right: 20px;
  cursor: pointer;
  z-index: 2;
}

.bar {
  height: 5px;
  width: 30px;
  background: #e1ecfa;
  border-radius: 5px;
  margin-bottom: 6px;
}

.close {
  margin: 10px;
}
.close .bar {
  width: 20px;
}
.close .bar:nth-child(1) {
  transform: rotate(45deg);
  position: absolute;
  margin: 0px;
}

.close .bar:nth-child(2) {
  transform: rotate(-45deg);
  margin: 0px;
}

.close .bar:nth-child(3) {
  display: none;
}

</style>
