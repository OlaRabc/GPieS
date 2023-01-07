<script setup>
import Soon from "./components/Soon.vue";
import Nav from "./components/Nav.vue";
import Footer from "./components/Footer.vue";
import Products from "./components/Products.vue";
import Main from "./components/Main.vue";

import { library } from "@fortawesome/fontawesome-svg-core";
import {faArrowDown} from '@fortawesome/free-solid-svg-icons'
</script>

<template>
  <div>
    <Nav />

    <div class="wrapper">
      <!-- <Soon /> -->
      <Products/>
      <!-- <Main /> -->
      <font-awesome-icon icon="fa-brands fa-facebook-f" />
      <faArrowDown/>
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
