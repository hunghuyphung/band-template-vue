<script setup>
import facebook from "@/assets/icons/facebook.svg";
import instagram from "@/assets/icons/instagram.svg";
import tikTok from "@/assets/icons/tik-tok.svg";
import pinterest from "@/assets/icons/pinterest.svg";
import twitter from "@/assets/icons/twitter.svg";
import linkedin from "@/assets/icons/linkedin.svg";

const socialMedias = [facebook, instagram, tikTok, pinterest, twitter, linkedin];
</script>

<template>
  <div class="p-64-16 text-center font-latos">
      <p>
        <img v-for="socialMedia in socialMedias" :src="socialMedia" alt=""  class="social-media-icon opacity-60">
      </p>
    <p class="m-15-0 opacity-60">Powered by w3.css</p>
  </div>
</template>

<style scoped>
  .social-media-icon {
    width: 1.25rem;
    margin: 0 0.25rem;
  }
</style>
