<script setup>
import Soon from "./components/Soon.vue";
import Nav from "./components/Nav.vue";
import Footer from "./components/Footer.vue";
import Products from "./components/Products.vue";
import Main from "./components/Main.vue";
import Login from "./components/Login.vue";


</script>

<template>
  <div>
    <Nav @changePage="changePage"/>

    <div class="wrapper">
      <Main v-if="page === 0" />
      <Products v-if="page === 1"/>
      <Login v-if="page === 2"/>

      <Soon v-if="page === 3"  @changePage="changePage"/>
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
      page: 0
    }
  },
  methods: {
    changePage(pageNumber) {
      this.page=pageNumber;
    },
  },
};
</script>