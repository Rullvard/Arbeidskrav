<template>
  <div class="home">
    <h1>{{ heading }}</h1>
    <Image image="nora1.jpg" />
  </div>
</template>

<script>
import Image from "../components/Image";

export default {
  name: "Home",
  components: {},
  setup() {
    return {
      Image,
      heading: "Nora En Pure",
    };
  },
};
</script>
