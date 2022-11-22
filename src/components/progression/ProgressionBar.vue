<template>
  <div class="progress-bar">
    <v-progress-linear v-model="recred" color="white" height="25">
      <!-- <div class="progress-value">{{ recred }}%</div> -->
    </v-progress-linear>
  </div>
</template>

<style>
.progress-bar {
  padding-left: 0.5vw;
  padding-right: 0.5vw;
}

/* .progress-value {
  color: white;
  text-align: center;
} */
</style>

<script lang="ts">
export default {
  name: "ProgressionBar",
  data: () => ({
    recred: 12,
  }),
};
</script>
