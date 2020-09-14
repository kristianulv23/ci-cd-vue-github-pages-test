<template>
  <div id="app">
    <base-button @on-click="onClick($event)" text="PRESS MY BUTTON"></base-button>
  </div>
</template>

<script>
import BaseButton from "./components/BaseButton.vue";

export default {
  name: "App",
  components: {
    BaseButton,
  },
  methods: {
    onClick: function (e) {
      console.log(e);
    },
  },
};
</script>

<style>
*,
*::before,
*::after {
  box-sizing: border-box;
}

html {
  font-size: 16px;
}

body {
  margin: 0;
}

#app {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
}
</style>
