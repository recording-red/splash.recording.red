<template>
  <div class="register">
    <input
      class="register-input"
      type="text"
      placeholder="Votre adresse eMail"
      v-model="email"
    />
    <img class="register-play" :src="src" />
  </div>
</template>

<style scoped>
.register {
  padding: 0em 0em 0em 2em;
}

.register-input {
  width: 25vw;
  max-width: 20em;
  min-width: 15em;
  font-size: x-large;
  background: transparent;
  color: white;
}

.register-play {
  width: 1.5em;
  position: absolute;
  bottom: 0.4vh;
  right: 0.25vw;
}
</style>

<script lang="ts">
import Src from "@/assets/play.png";

export default {
  name: "Register",

  data: () => ({
    src: Src,
    email: "",
  }),
};
</script>
