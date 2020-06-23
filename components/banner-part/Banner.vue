<template>
  <div class="main-wrapper">
    <img src="https://thehub.io/_nuxt/img/5797eb4.jpg" alt />
    <Input />
    <Imagepatern />
  </div>
</template>

<script>
import Imagepatern from "./Imagepatern";
import Input from "./Input";
export default {
  components: {
    Imagepatern,
    Input
  }
};
</script>

<style lang="scss" scoped>
.main-wrapper {
  margin-top: 150px;
  display: flex;
  justify-content: center;
  @media only screen and (max-width: 768px) {
    margin-top: 150px;
  }
}
img {
  width: 100vw;
  position: absolute;
  z-index: -100;
  @media only screen and (max-width: 768px) {
    width: 100vw;
    height: 250px;
    margin-top: 150px;
  }
}
</style>