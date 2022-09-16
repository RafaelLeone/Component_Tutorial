<template>
  <button
    class="b-button"
    :class="{
      [`b-button--color-${color}`]: true,
    }"
  >
    <slot />
  </button>
</template>

<script>
export default {
  props: {
    color: {
      type: String,
      default: "primary",
    },
  },
};
</script>

<style>
.b-button {
  text-decoration: none;
  z-index: 92;
  background-image: none;
  color: rgb(255, 255, 255);
  border: 0px;
  font-size: 17.6659px;
  text-align: center;
  border-radius: 100px;
  padding-left: 28px;
  padding-right: 28px;
  padding-top: 5px;
  padding-bottom: 5px;
}
.b-button--color-primary {
  background-color: rgb(241, 16, 117);
}
.b-button--color-secondary {
  background-color: rgb(136, 2, 214);
}
</style>
