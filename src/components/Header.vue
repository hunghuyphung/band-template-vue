<script setup>
import search from "@/assets/icons/search.svg";
</script>

<template>
  <header id="header" class="flex justify-between bc-black">
    <div>
      <a href="#" class="inline-block p-12-24 text-white uppercase font-latos hover-grey">Home</a>
      <a href="#" class="inline-block p-12-24 text-white uppercase font-latos hover-grey">Band</a>
      <a href="#" class="inline-block p-12-24 text-white uppercase font-latos hover-grey">Tour</a>
      <a href="#" class="inline-block p-12-24 text-white uppercase font-latos hover-grey">Contact</a>
      <a href="#" class="inline-block p-12-24 text-white uppercase font-latos hover-grey">More</a>
    </div>
    <img :src="search" alt="" class="h-full header-search p-12-24">
  </header>
</template>

<style scoped>
#header {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1;
  height: var(--header-height);
}

.p-12-24 {
  padding: 0.75rem 1.5rem;
}

.header-search {
  max-width: 3.875rem;
}

.header-search:hover {
  background-color: var(--red);
  cursor: pointer;
}
</style>
