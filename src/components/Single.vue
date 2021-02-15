<template>
  <section>
    <div class="single-wrap">
      <h3>{{ singleTitle }}</h3>
      <img
        class="cover-img"
        :src="require(`@/assets/${image}`)"
        @click="toggleModal"
      />
      <p>{{ releaseYear }}</p>
    </div>
  </section>
</template>

<script>
import Modal from "../components/Modal";

export default {
  components: { Modal },
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
.cover-img {
  max-width: 322px;
}
</style>