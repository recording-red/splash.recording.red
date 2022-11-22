<!-- https://next.vuetifyjs.com/en/components/images/ -->

<template>
  <!-- // LogoHiragino.png -->
  <v-img class="logo" :src="src" />
</template>

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
