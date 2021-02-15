<template>
  <div class="singles">
    <Single
      v-for="(single, index) in singles"
      :key="index"
      :singleTitle="single.singleTitle"
      :releaseYear="single.releaseYear"
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
      { singleTitle: "Wetlands", releaseYear: "2020", image: "wetlands.jpg" },
      { singleTitle: "Delta", releaseYear: "2020", image: "delta.jpg" },
      {
        singleTitle: "All I Need",
        releaseYear: "2020",
        image: "all-i-need.jpg",
      },
      {
        singleTitle: "In Your Eyes",
        releaseYear: "2020",
        image: "in-your-eyes.jpg",
      },
      {
        singleTitle: "Come Away",
        releaseYear: "2020",
        image: "come-away.jpg",
      },
      {
        singleTitle: "Enchantment",
        releaseYear: "2021",
        image: "ench.jpg",
      },
    ]);
    return { Single, singles };
  },
};
</script>

<style>
.singles {
  display: grid;
  grid-template-columns: auto auto auto;
}
</style>