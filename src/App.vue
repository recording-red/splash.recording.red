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
</template>

<style>
.myapp {
  width: 100vw;
  min-width: 100vw;
  height: 100vh;
  min-height: 100vh;
}

.container {
  display: flex;
  flex-direction: column;
}

.debug {
  background-color: white;
  opacity: 50%;
}
</style>

<script setup lang="ts">
import Progression from "@/components/progression/Progression.vue";
import Footer from "./components/footer/Footer.vue";

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
