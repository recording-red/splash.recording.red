<template>
  <div
    class="myapp"
    v-bind:style="{
      backgroundImage: 'url(' + randomImgSrc + ')',
      backgroundSize: 'cover',
      backgroundRepeat: 'no-repeat',
    }"
  >
    <Progression />
  </div>
  <FollowUs />
</template>

<style scoped>
.myapp {
  width: 100vw;
  min-width: 100vw;
  height: 100vh;
  min-height: 100vh;
}
</style>

<script setup lang="ts">
import Progression from "@/components/progression/Progression.vue";
import FollowUs from "./components/follow_us/FollowUs.vue";

function getRandomInt(max: number): number {
  return Math.floor(Math.random() * max) + 1;
}

function addLeadingZeros(num: number, totalLength: number): string {
  return String(num).padStart(totalLength, "0");
}

function randomImage() {
  let nb = getRandomInt(17);
  return "/backgrounds/" + addLeadingZeros(nb, 3) + ".jpg";
}

const randomImgSrc = randomImage();
</script>
