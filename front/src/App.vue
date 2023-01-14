<script setup>
import Nav from "./components/Nav.vue";
import NavLogged from "./components/NavLogged.vue";
import Footer from "./components/Footer.vue";

import Soon from "./components/Soon.vue";
import Products from "./components/Products.vue";
import Main from "./components/Main.vue";
import Login from "./components/Login.vue";
import Map from "./components/Map.vue";



</script>

<template>
  <div>
    <Nav v-if="!log" @changePage="changePage"/>
    <NavLogged v-if="log" @changePage="changePage"/>
    <div class="wrapper">
      <Main v-if="page === 0" />
      <Products v-if="page === 1"/>
      <Login v-if="page === 2" @changePage="changePage"/>
      <Soon v-if="page === 3"  @changePage="changePage"/>
      <Map v-if="page === 4"/>

    </div>

    <Footer />
  </div>
</template>

<style scoped>
</style>

<script>
export default {
  data() {
    return {
      page: 0,
      log: false
    }
  },
  methods: {
    changePage(pageNumber) {
      if(pageNumber===4)  this.log = true;
      else this.log = false;
      this.page=pageNumber;
    },
  },
};
</script>