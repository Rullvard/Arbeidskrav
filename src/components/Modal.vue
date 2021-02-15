<template>
  <div class="backdrop" @click.self="closeModal">
    <div class="modal">
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    closeModal() {
      this.$emit("close");
    },
  },
};
</script>


// scoped makes the styling only affect the component itself
<style>
.backdrop {
  top: 0;
  left: 0;
  position: fixed;
  background: rgba(0, 0, 0, 0.5);
  width: 100%;
  height: 100%;
}

.modal {
  width: 600px;
  padding: 20px;
  margin: 50px auto;
  background: #394453;
  border-radius: 10px;
}
</style>