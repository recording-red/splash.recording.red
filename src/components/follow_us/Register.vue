<template>
  <div class="register">
    <input
      class="register-input"
      type="email"
      pattern=".+@.+\..+"
      placeholder="Votre adresse eMail"
      v-model="email"
      v-on:keyup.enter="saveEmail"
    />
    <img class="register-play" :src="src" @click="saveEmail" />
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
    ip: "",
  }),

  async mounted() {
    const response = await fetch("https://api.ipify.org");
    //const { data: ip } = await response.json()
    this.ip = await response.text();
  },

  methods: {
    async saveEmail() {
      const data = {
        email: this.email,
        ip: this.ip,
      };

      const response = await fetch(import.meta.env.VITE_RECRED_URL + "/registration/", {
        method: "POST", // *GET, POST, PUT, DELETE, etc.
        mode: "cors", // no-cors, *cors, same-origin
        cache: "no-cache", // *default, no-cache, reload, force-cache, only-if-cached
        headers: {
          "Content-Type": "application/json",
          // 'Content-Type': 'application/x-www-form-urlencoded',
        },
        redirect: "follow", // manual, *follow, error
        referrerPolicy: "no-referrer", // no-referrer, *no-referrer-when-downgrade, origin, origin-when-cross-origin, same-origin, strict-origin, strict-origin-when-cross-origin, unsafe-url
        body: JSON.stringify(data),
      });
      this.email = "";
    },
  },
};
</script>
