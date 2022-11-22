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
import Src from "@/assets/social/facebook_white.png";

export default {
  name: "Facebook",

  data() {
    return {
      src: Src,
    };
  },
};
</script>
