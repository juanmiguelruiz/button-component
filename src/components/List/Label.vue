<template>
  <label>&lt;{{ text }} /&gt;</label>
</template>

<script>
export default {
  name: "Label",
  props: {
    text: {
      type: String,
      default: "",
    },
  },
};
</script>

<style>
label {
  font-family: "Courier New", Courier, monospace;
  font-size: 14px;
  line-height: 12px;
  color: #333333;
}
</style>
