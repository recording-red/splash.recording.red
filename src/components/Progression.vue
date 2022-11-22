<template>
  <div class="flex-container">
    <div class="row">
      <div class="flex-item"><Logo /></div>
      <div class="flex-item"><ProgressionBar /></div>
      <div class="flex-item"><ProgressionValue /></div>
    </div>
  </div>
</template>

<style>
.flex-container {
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}
.row {
  width: 800px;
}
.flex-item {
  text-align: center;
  margin-bottom: 30px;
}
</style>

<script lang="ts">
import Logo from "@/components/Logo.vue";
import ProgressionBar from "@/components/ProgressionBar.vue";
import ProgressionValue from "@/components/ProgressionValue.vue";

export default {
  name: "Progression",

  components: { Logo, ProgressionBar, ProgressionValue },
};
</script>
