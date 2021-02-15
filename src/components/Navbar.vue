<template>
  <div id="nav" class="flexbox-container">
    <div class="flex-item-1">
      <router-link :to="{ name: 'Home' }"
        ><img src="../assets/logo.png"
      /></router-link>
    </div>
    <div class="flex-item-2">
      <router-link :to="{ name: 'About' }">About</router-link>
      <router-link :to="{ name: 'Contact' }">Contact</router-link>
      <router-link :to="{ name: 'Music' }">Music</router-link>
    </div>
    <div v-if="showModal">
      <Modal @close="toggleModal">
        <BuyTicket />
      </Modal>
    </div>
    <button @click="toggleModal">Buy Tickets</button>
  </div>
</template>

<script>
import Modal from "./Modal.vue";
import BuyTicket from "./BuyTicket.vue";

export default {
  components: {
    Modal,
    BuyTicket,
  },
  data() {
    return {
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
.flexbox-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

#nav {
  padding: 30px;
  background: #0b2238;
}

#nav img {
  height: 50px;
}

#nav a,
button {
  font-weight: bold;
  text-decoration: none;
  color: #f3f3f3;
  margin: 0 20px;
  font-size: 16px;
}

button {
  background: #0b2238;
  border: 2px solid #f3f3f3;
  padding: 8px 18px;
  cursor: pointer;
}
</style>