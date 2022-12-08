<template>
  <div class="progress-bar">
    <div class="progress-bar-value" />
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
