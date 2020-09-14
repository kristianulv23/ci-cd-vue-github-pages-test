<template>
  <button @click="onClick">{{text}}</button>
</template>


<script>
export default {
  name: "base-button",
  props: {
    text: {
      type: String,
    },
  },
  methods: {
    onClick: function (e) {
      this.$emit("on-click", e);
    },
  },
};
</script>

<style scoped>
button {
  background: rgb(98, 126, 98);
  border: none;
  color: white;
  padding: 1em 2em;
  border-radius: 50px;
  font-size: 1.5em;
  cursor: pointer;
  box-shadow: 3px 3px 10px 2px lightgrey;
}
</style>