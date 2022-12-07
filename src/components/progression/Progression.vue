<template>
  <div class="flex-container">
    <div class="flex-item"><Logo /></div>
    <div class="flex-item"><ProgressionBar /></div>
    <div class="flex-item"><ProgressionValue /></div>
  </div>
</template>

<style scoped>
.flex-container {
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
</style>

<script lang="ts">
import Logo from "@/components/progression/Logo.vue";
import ProgressionBar from "@/components/progression/ProgressionBar.vue";
import ProgressionValue from "@/components/progression/ProgressionValue.vue";

export default {
  name: "Progression",

  components: { Logo, ProgressionBar, ProgressionValue },
};
</script>
