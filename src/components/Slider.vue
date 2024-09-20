<script setup>
import ny from '@/assets/imgs/ny.jpg';
import chicago from '@/assets/imgs/chicago.jpg';
import la from '@/assets/imgs/la.jpg';
import {ref} from "vue";

const sliders = [
  {
    location: 'New York',
    intro: 'The atmosphere in New York is lorem ipsum.',
    img: ny
  },
  {
    location: 'Chicago',
    intro: 'Thank you, Chicago - A night we won\'t forget.',
    img: chicago
  },
  {
    location: 'Los Angeles',
    intro: 'We had the best time playing at Venice Beach!',
    img: la
  }
];

const currentSlideIndex = ref(0);

setInterval(() => {
  currentSlideIndex.value = currentSlideIndex.value < 2 ? currentSlideIndex.value + 1 : 0;
}, 4000);

</script>

<template>
  <div id="slider" class="relative">
    <img :src="sliders[currentSlideIndex].img" alt="" class="block w-full">
    <div class="slider__content w-full text-center text-white">
      <h3>{{ sliders[currentSlideIndex].location }}</h3>
      <p class="m-15-0"><b class="font-latos">{{ sliders[currentSlideIndex].intro }}</b></p>
    </div>
  </div>
</template>

<style scoped>
.slider__content {
  position: absolute;
  bottom: 2rem;
}
</style>
