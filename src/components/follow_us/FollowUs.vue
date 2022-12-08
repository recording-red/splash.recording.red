<template>
  <div class="follow-us">
    <FollowUsText />
    <Share />
    <!-- <Share style="padding:1em 2.5em 0em 0em;"/> -->
  </div>
</template>

<style scoped>
.follow-us {
  position: absolute;
  bottom: 3vh;
  right: 3vw;
  text-align: right;
}
</style>

<script lang="ts">
import FollowUsText from "@/components/follow_us/FollowUsText.vue";
import Share from "@/components/follow_us/Share.vue";

export default {
  name: "FollowUs",
  components: { FollowUsText, Share },
};
</script>
