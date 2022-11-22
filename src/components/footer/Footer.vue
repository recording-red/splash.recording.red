<template>
  <div class="footer">
    <FooterText />
    <Share />
  </div>
</template>

<style>
.footer {
  position: absolute;
  bottom: 3vh;
  right: 3vw;
}
</style>

<script lang="ts">
import FooterText from "@/components/footer/FooterText.vue";
import Share from "@/components/footer/Share.vue";

export default {
  name: "Footer",
  components: { FooterText, Share },
};
</script>
