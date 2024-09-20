<script setup>
import bandmember from "@/assets/imgs/bandmember.jpg";

const bandMember = {
  name: 'Name',
  avatar: bandmember
};

const bandMembers = Array(3).fill(bandMember);
</script>

<template>
  <div class="mx-auto p-64-16 max-w-800 bc-white text-center">
    <h2 class="tracking-4">THE BAND</h2>
    <p class="m-15-0"><i class="font-latos opacity-40">We love music</i></p>
    <p class="m-15-0 text-justify font-latos">We have created a fictional band website. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
    <div class="p-32-0 flex">
      <div v-for="b in bandMembers">
        <p class="m-15-0 font-latos">{{b.name}}</p>
        <img :src="b.avatar" alt="" class="mx-auto mb-15 block w-60 rounded-4">
      </div>
    </div>
  </div>
</template>

<style scoped>
.rounded-4 {
  border-radius: 0.25rem;
}

.mb-15 {
  margin-bottom: 15px;
}
</style>
