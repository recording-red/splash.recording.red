<template>
  <div class="share-logo">
    <v-img :src="src" />
  </div>
</template>

<style>
.share-logo {
  width: 2.5em;
}
</style>

<script lang="ts">
import Src from "@/assets/social/instagram_white.png";

export default {
  name: "Instagram",

  data() {
    return {
      src: Src,
    };
  },
};
</script>
