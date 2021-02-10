<template>
  <div id="nav">
    <router-link class="logo" :to="{ name: 'Home' }"
      ><img src="../assets/logo.png"
    /></router-link>
    <router-link :to="{ name: 'About' }">About</router-link>
    <router-link :to="{ name: 'Contact' }">Contact</router-link>
    <router-link :to="{ name: 'Music' }">Music</router-link>
  </div>
</template>

<script>
export default {};
</script>

<style>
#nav {
  padding: 30px;
  background: #0b2238;
}

#nav a {
  font-weight: bold;
  text-decoration: none;
  color: #f3f3f3;
  padding: 15px;
}

#nav img {
  width: 70px;
}
</style>