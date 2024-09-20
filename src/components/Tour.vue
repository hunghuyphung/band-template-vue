<script setup>
import newyork from '@/assets/imgs/newyork.jpg';
import paris from '@/assets/imgs/paris.jpg';
import sanfran from '@/assets/imgs/sanfran.jpg';

const tours = [
  {
    id: 1,
    location: 'New York',
    performanceDate: 'Fri 27 Nov 2016',
    intro: 'Praesent tincidunt sed tellus ut rutrum sed vitae justo.',
    img: newyork
  },
  {
    id: 2,
    location: 'Paris',
    performanceDate: 'Sat 28 Nov 2016',
    intro: 'Praesent tincidunt sed tellus ut rutrum sed vitae justo.',
    img: paris
  },
  {
    id: 3,
    location: 'San Francisco',
    performanceDate: 'Sun 29 Nov 2016',
    intro: 'Praesent tincidunt sed tellus ut rutrum sed vitae justo.',
    img: sanfran
  }
];
</script>

<template>
  <div class="bc-black">
    <div class="mx-auto p-64-16 max-w-800 text-center text-white">
      <h2 class="tracking-4">TOUR DATES</h2>
      <p class="m-15-0"><i class="font-latos opacity-40">Remember to book your tickets!</i></p>
      <br>
      <ul class="text-justify font-latos">
        <li class="p-8-16 block bc-white text-light-grey">September <span class="ml-16 p-0-8 inline-block bc-red text-white">Sold out</span></li>
        <li class="p-8-16 block bc-white text-light-grey">October <span class="ml-16 p-0-8 inline-block bc-red text-white">Sold out</span></li>
        <li class="p-8-16 flex justify-between bc-white text-light-grey">November <span class="ml-16 p-0-8 inline-block rounded-half bc-black text-white">3</span></li>
      </ul>
      <div class="mx-negative-16 p-32-0 flex">
          <div v-for="tour in tours" :key="tour.id" class="mb-16 p-0-8">
            <img :src="tour.img" alt="" class="block w-full hover-opacity">
            <div class="p-0-16 bc-white text-justify text-black font-latos clearfix">
              <p class="m-15-0"><b>{{ tour.location }}</b></p>
              <p class="m-15-0 opacity-60">{{ tour.performanceDate }}</p>
              <p class="m-15-0 text-justify">{{ tour.intro }}</p>
              <button class="mb-15 button bc-black text-white font-latos hover-grey">
                Buy Tickets
              </button>
            </div>
          </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
li {
  border-bottom: 1px solid #ddd;
}

.bc-red {
  background-color: var(--red);
}

.rounded-half {
  border-radius: 50%;
}

.p-8-16 {
  padding: 0.5rem 1rem;
}

.mb-15 {
  margin-bottom: 15px;
}

.ml-16 {
  margin-left: 1rem;
}

.mb-16 {
  margin-bottom: 1rem;
}
</style>
