<template>
  <div class="share">
    <Facebook class="share-block" />
    <Instagram class="share-block" />
    <Twitter class="share-block" />
    <Tiktok class="share-block" />
    <Linkedin class="share-block" />
    <Youtube class="share-block" />
    <Register class="share-block" />
  </div>
</template>

<style>
.share {
  position: relative;
  float: right;
  display: inline;
}

.share-block {
  display: inline-block;
}
</style>

<script lang="ts">
import Facebook from "@/components/footer/Facebook.vue";
import Instagram from "@/components/footer/Instagram.vue";
import Twitter from "@/components/footer/Twitter.vue";
import Tiktok from "@/components/footer/Tiktok.vue";
import Linkedin from "@/components/footer/Linkedin.vue";
import Youtube from "@/components/footer/Youtube.vue";
import Register from "@/components/footer/Register.vue";

export default {
  name: "Share",

  components: {
    Facebook,
    Instagram,
    Twitter,
    Tiktok,
    Linkedin,
    Youtube,
    Register,
  },
};
</script>
