<template>
  <div class="social-media-wrapper">
    <a :href="url" target="”_blank”"
      ><img class="social-media-logo" :src="logo"
    /></a>
  </div>
</template>

<style scoped>
.social-media-logo {
  height: 1.5em;
  padding: 0em 0em 0em 2em;
}
</style>

<script lang="ts">
import Src from "@/assets/social/facebook_white.png";

export default {
  name: "SocialMedia",

  props: {
    logo: String,
    url: String,
  },

  data() {
    return {
      src: Src,
    };
  },
};
</script>
