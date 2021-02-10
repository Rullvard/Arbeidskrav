<template>
  <h1>{{ title }}</h1>
  <div v-if="showModal">
    <Modal @close="toggleModal">
      <h3>{{ title }}</h3>
      <p>{{ text }}</p>
    </Modal>
  </div>
  <button @click="toggleModal">Show Modal</button>
</template>


<script>
import Modal from "../components/Modal.vue";

export default {
  name: "App",
  components: {
    Modal,
  },
  data() {
    return {
      title: "My Vue App",
      text: "Grab your tickets now",
      showModal: false,
    };
  },
  methods: {
    toggleModal() {
      this.showModal = !this.showModal;
    },
  },
};
</script>

<style>
</style>