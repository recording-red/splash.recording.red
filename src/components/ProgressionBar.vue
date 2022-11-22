<template>
  <div class="progress-bar">
    <v-progress-linear v-model="recred" color="white" height="25">
    </v-progress-linear>
  </div>
</template>

<style>
.progress-bar {
  padding-left: 10px;
  padding-right: 10px;
}
</style>

<script lang="ts">
export default {
  name: "ProgressionBar",
  data: () => ({
    recred: 12,
  }),
};
</script>
