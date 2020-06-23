<template>
  <img :src="img" alt />
</template>

<script>
export default {
  name: "Categoryimg",
  props: ["img"]
};
</script>

<style lang="scss" scoped>
img {
  position: absolute;
  z-index: -10;
  @media only screen and (max-width: 768px) {
    display: none;
  }
  @media only screen and (max-width: 1250px) {
    display: none;
  }
}
.img-startup {
  left: 30px;
  margin-top: 450px;
  width: 5vw;
  @media only screen and (min-width: 1250px) and (max-width: 1620px) {
    left: 150px;
  }
}
.img-category {
  left: 280px;
}
</style>