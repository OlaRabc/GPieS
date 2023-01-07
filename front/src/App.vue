<script setup>
import Soon from "./components/Soon.vue";
import Nav from "./components/Nav.vue";
import Footer from "./components/Footer.vue";
import Products from "./components/Products.vue";
import Main from "./components/Main.vue";

</script>

<template>
  <div>
    <Nav @changePage="changePage"/>

    <div class="wrapper">
      <Main v-if="page === 0" />
      <Products v-if="page === 1"/>
      <Soon v-if="page === 3"  @changePage="changePage"/>
    </div>

    <Footer />
  </div>
</template>

<style scoped>
footer {
  background-color: #495f7a;
  height: 150px;
  position: relative;
  height: 190px;
}
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