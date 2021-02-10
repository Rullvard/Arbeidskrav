<template>
  <img :src="require(`@/assets/${image}`)" />
</template>

<script>
export default {
  props: {
    image: {
      type: String,
      default: "logo.png",
    },
  },
};
</script>

<style>
</style>