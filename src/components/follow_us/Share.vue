<template>
  <div class="share-wrapper">
    <SocialMedia
      class="share-content"
      logo="/social/facebook.png"
      url="https://www.facebook.com"
    />
    <SocialMedia
      class="share-content"
      logo="/social/instagram.png"
      url="https://www.instagram.com"
    />
    <SocialMedia
      class="share-content"
      logo="/social/twitter.png"
      url="https://www.twitter.com"
    />
    <SocialMedia
      class="share-content"
      logo="/social/tiktok.png"
      url="https://www.tiktok.com"
    />
    <SocialMedia
      class="share-content"
      logo="/social/linkedin.png"
      url="https://www.linkedin.com"
    />
    <SocialMedia
      class="share-content"
      logo="/social/youtube.png"
      url="https://www.youtube.com"
    />
    <Register class="share-content" />
  </div>
</template>

<style scoped>
.share-wrapper {
  padding-top: 1em;
}

.share-content {
  display: inline-block;
}
</style>

<script lang="ts">
import SocialMedia from "@/components/follow_us/SocialMedia.vue";
import Register from "@/components/follow_us/Register.vue";

export default {
  name: "Share",

  components: {
    Register,
    SocialMedia,
  },
};
</script>
