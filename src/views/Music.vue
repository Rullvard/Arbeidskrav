<template>
  <section>
    <div class="content-wrap">
      <h2>New Releases</h2>
      <SingleList />
    </div>
  </section>
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
h2 {
  padding: 40px;
  font-size: 34px;
}

h3 {
  padding: 8px;
  text-align: center;
  font-size: 22px;
}

p {
  font-size: 16px;
  padding: 0.5em 0 3.5em 0;
}
</style>