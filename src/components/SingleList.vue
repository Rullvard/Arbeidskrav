<template>
  <div>
    <Single
      v-for="(single, index) in singles"
      :key="index"
      :singleTitle="single.singleTitle"
      :releaseDate="single.releaseDate"
      :image="single.image"
    />
  </div>
</template>

<script>
import { ref } from "vue";
import Single from "./Single";

export default {
  setup() {
    const singles = ref([
      { singleTitle: "Wetlands", releaseDate: "2020", image: "wetlands.jpg" },
      { singleTitle: "Delta", releaseDate: "2020", image: "delta.jpg" },
      {
        singleTitle: "All I Need",
        releaseDate: "2020",
        image: "all-i-need.jpg",
      },
    ]);
    return { Single, singles };
  },
};
</script>

<style>
</style>