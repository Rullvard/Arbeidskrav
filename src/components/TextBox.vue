<template>
  <div class="text-box" :class="{ contact: theme === 'contact' }">
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: ["theme"],
};
</script>

<style>
.text-box {
  background: #0b2238;
  width: 45%;
  border: 1px solid white;
  padding: 40px;
  margin-right: 20px;
}

.text-box.contact {
  width: 40%;
  margin: 40px auto;
}
.text-box.contact p {
  padding: 10px;
}

.text-box.contact h2 {
  padding-top: 10px;
}
</style>