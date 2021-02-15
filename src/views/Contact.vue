<template>
  <div class="contact">
    <div class="hero">
      <Image image="contact-hero.jpg" />
    </div>
    <TextBox theme="contact">
      <h2>Contact me</h2>
      <div class="contact-info">
        <p>For booking: booking@noramail.com</p>
        <p>Licensing: licensing@noramial.com</p>
      </div>
    </TextBox>
  </div>
</template>

<script>
import TextBox from "../components/TextBox.vue";
import Image from "../components/Image.vue";
export default {
  components: {
    TextBox,
    Image,
  },
};
</script>

<style>
.hero img {
  object-fit: cover;
  width: 100%;
  height: 250px;
}

.contact-info {
  padding-bottom: 20px;
}
</style>