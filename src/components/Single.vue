<template>
  <h3>{{ singleTitle }}</h3>
  <img :src="require(`@/assets/${image}`)" />
  <p>{{ releaseYear }}</p>
</template>

<script>
export default {
  props: {
    singleTitle: String,
    releaseYear: String,
    image: {
      type: String,
      default: "logo.png",
    },
  },
};
</script>

<style>
</style>