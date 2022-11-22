<template>
  <form class="form">
    <input type="text" placeholder="Votre adresse e-mail" />
    <button class="button" type="submit">
      <img class="img" :src="src" alt="Search" />
    </button>
  </form>
</template>

<style>
.form {
  display: inline-block;
  border: 1px solid #ccc;
  min-width: 30em;
  max-height: 2.5em;
  color: white;
  position: relative;
  bottom: 0.6em;
}

.form input {
  border: none;
  padding-left: 0.2em;
  position: relative;
  bottom: 0.4em;
  min-width: 30em;
  max-height: 2.5em;
  color: white;
}

.img {
  width: 1.2em;
  position: relative;
  bottom: 0.1em;
  left: 0.7em;
}
</style>

<script lang="ts">
import Src from "@/assets/play.png";

export default {
  name: "Register",

  data: () => ({
    src: Src,
  }),
};
</script>
