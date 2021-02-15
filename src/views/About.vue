<template>
  <h1>About</h1>
  <div class="flex-box">
    <TextBox theme="">
      <h2>Nora En Pure</h2>
      <p>
        Daniela Di Lillo (formerly Niederer, born 20 July 1990), better known by
        her stage name Nora En Pure, is a South African-Swiss DJ and deep
        house producer. She first received recognition for her 2013 single "Come
        With Me". Further popular releases are "Morning Dew", "Lake Arrowhead",
        and "Tears In Your Eyes." In July 2016, she was invited to put together
        a two-hour long mix for Pete Tong's radio show: "BBC's Essential Mix".
      </p>
    </TextBox>
    <Image image="nora2.jpg" />
  </div>
</template>

<script>
import Image from "../components/Image.vue";
import TextBox from "../components/TextBox";

export default {
  components: {
    TextBox,
    Image,
  },
};
</script>

<style>
.flex-box {
  display: flex;
  margin: 4%;
  justify-content: space-between;
}
</style>