<script setup>

import Slider from "@/components/Slider.vue";
import Header from "@/components/Header.vue";
import Band from "@/components/Band.vue";
import Tour from "@/components/Tour.vue";
import Contact from "@/components/Contact.vue";
import Footer from "@/components/Footer.vue";
</script>

<template>
  <Header></Header>
  <div id="container">
    <Slider></Slider>
    <Band></Band>
    <Tour></Tour>
    <Contact></Contact>
    <Footer></Footer>
  </div>
</template>

<style scoped>
  #container {
    margin-top: var(--header-height);
  }
</style>
