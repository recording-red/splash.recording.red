<template>
  <!-- <div class="progress-bar"> -->
  <!-- <div class="progress-bar-total">&nbsp;</div>
    <div class="progress-bar-current">&nbsp;</div> -->
  <!-- <progress class="progress" :value="progression" max="100">32%</progress> -->
  <!-- </div> -->
  <div class="progress-bar">
    <!-- <div class="progress-bar-value" style="height: 24px; width: 25%"></div> -->
    <div class="progress-bar-value"></div>
  </div>
  <br />
</template>

<style lang="scss" scoped>
@import "src/assets/style.scss";

.progress-bar {
  width: 45vw;
  height: 2vh;
  background-color: $color-dark-grey;
  opacity: 60%;
}

.progress-bar-value {
  background-color: $color-white;
  width: 12%;
  height: 2vh;
}
</style>

<script lang="ts">
export default {
  name: "ProgressionBar",
  data: () => ({
    progression: 12,
  }),
};
</script>
