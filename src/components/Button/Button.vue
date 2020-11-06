<template>
  <button
    :class="[
      size,
      variant,
      color,
      { 'disable-sahdow': disableShadow, disabled: disabled },
    ]"
    :disabled="{ disabled }"
  >
    <span class="material-icons" v-if="startIcon">{{ startIcon }}</span>
    <p v-if="disbled">Disabled</p>
    <p v-else>{{ text }}</p>
    <span class="material-icons" v-if="endIcon">{{ endIcon }}</span>
  </button>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: {
      type: String,
      default: "Default",
    },
    size: {
      type: String,
      default: "md",
      validator: function(value) {
        return ["sm", "md", "lg"].indexOf(value) !== -1;
      },
      variant: {
        type: String,
        default: "",
        validator: function(value) {
          return ["", "outline", "text"].indexOf(value) !== -1;
        },
      },
    },
    color: {
      type: String,
      default: "default",
      validator: function(value) {
        return (
          ["default", "primary", "secondary", "danger"].indexOf(value) !== -1
        );
      },
    },
    startIcon: String,
    endIcon: String,
    disabled: {
      type: Boolean,
      default: false,
    },
    disableShadow: Boolean,
  },
};
</script>

<style src="./styles.css" scoped />
