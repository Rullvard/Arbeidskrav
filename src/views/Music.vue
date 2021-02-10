<template>
  <h3>New Releases</h3>
  <div>
    <SingleList />
  </div>
</template>

<script>
import SingleList from "../components/SingleList";

export default {
  components: { SingleList },
  setup() {
    return { SingleList };
  },
};
</script>

<style>
</style>