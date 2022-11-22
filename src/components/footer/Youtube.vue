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
import Src from "@/assets/social/youtube_white.png";

export default {
  name: "Youtube",

  data() {
    return {
      src: Src,
    };
  },
};
</script>
