<script setup>
import marker from "@/assets/icons/marker.svg";
import envelope from "@/assets/icons/envelope.svg";
import phoneCall from "@/assets/icons/phone-call.svg";
import map from "@/assets/imgs/map.jpg";
</script>

<template>
  <div class="mx-auto p-64-16 max-w-800 bc-white text-center">
    <h2 class="tracking-4">CONTACT</h2>
    <p class="m-15-0"><i class="font-latos opacity-40">Fan? Drop a note!</i></p>
    <div class="p-32-0 flex">
      <div class="w-50 text-justify font-latos">
        <p class="text-lg">
          <img :src="marker" alt="" style="width: 1rem" class="mr-14">
          Chicago, US
        </p>
        <p class="text-lg">
          <img :src="phoneCall" alt="" style="width: 1rem" class="mr-14">
          Phone: +00 151515
        </p>
        <p class="text-lg">
          <img :src="envelope" alt="" style="width: 1rem" class="mr-14">
          Email: mail@mail.com
        </p>
      </div>
      <div class="w-50">
        <div class="flex mx-negative-16 mb-8">
          <div class="p-0-8">
            <input type="text" class="input" placeholder="Name">
          </div>
          <div class="p-0-8">
            <input type="text" class="input" placeholder="Email">
          </div>
        </div>
        <input type="text" class="input" placeholder="Message">
        <div class="m-15-0 flex justify-end">
          <button class="mb-15 button bc-black text-white font-latos hover-grey">
            SEND
          </button>
        </div>
      </div>
    </div>
  </div>
  <img :src="map" alt="" class="block w-full grayscale-min">
</template>

<style scoped>
.mb-8 {
  margin-bottom: 0.5rem;
}

.mr-14 {
  margin-right: 0.875rem;
}
</style>
