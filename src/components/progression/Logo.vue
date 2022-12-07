<template>
  <!-- // LogoHiragino.png -->
  <img class="logo" :src="src" />
</template>

<style>
.logo {
  width: 45vw;
  margin-bottom: 2vh;
}
</style>

<script lang="ts">
import Src from "@/assets/logo.png";

export default {
  name: "Logo",

  data() {
    return {
      src: Src,
    };
  },
};
</script>
