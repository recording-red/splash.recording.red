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
import Src from "@/assets/social/twitter_white.png";

export default {
  name: "Twitter",

  data() {
    return {
      src: Src,
    };
  },
};
</script>
