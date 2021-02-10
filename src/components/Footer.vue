<template>
  <footer>
    <div class="some">
      <a href="#"><i class="fab fa-facebook-f"></i></a>
      <a href="#"><i class="fab fa-instagram"></i></a>
      <a href="#"><i class="fab fa-twitter"></i></a>
      <a href="#"><i class="fab fa-soundcloud"></i></a>
      <a href="#"><i class="fab fa-spotify"></i></a>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style>
footer {
  position: fixed;
  left: 0;
  bottom: 0;
  width: 100%;
  padding: 15px;
  background: #0b2238;
}

footer .some {
  font-size: 1.5em;
}

footer .some i {
  color: rgb(0, 0, 0, 0.8);
  padding: 0 15px;
  color: #f3f3f3;
}
</style>