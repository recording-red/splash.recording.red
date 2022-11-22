<template>
  <div
  :style="{'background-image': randomImage()}"
  
  >AAA</div>

</template>

<style>
body {
  background: #ebeff0 no-repeat fixed center;
  background-image: url("/backgrounds/001.jpg");
  background-size: 100% 100%;
}
</style>

<script setup lang="ts">
function getRandomInt(max: number): number {
  return Math.floor(Math.random() * max) + 1;
}

function addLeadingZeros(num: number, totalLength: number): string {
  return String(num).padStart(totalLength, '0');
}

function randomImage() {
  let nb = getRandomInt(17);
  return "/backgrounds/" + addLeadingZeros(nb, 3) + ".jpg";
}

</script>
