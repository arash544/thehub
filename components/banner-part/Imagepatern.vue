<template>
  <div class="wrapper">
    <img src="https://thehub.io/_nuxt/8ff8f5e5964d29aaff07e332d9028534.svg" alt />
  </div>
</template>

<script>
export default {
  name: "Imagepatern"
};
</script>

<style lang="scss" scoped>
.wrapper {
  margin-top: -120px;
  width: 90%;
  display: flex;
  justify-content: flex-start;
  @media only screen and (max-width: 768px) {
    margin-top: -200px;
  }
}
img {
  width: 27vw;
  @media only screen and (max-width: 768px) {
    width: 50vw;
  }
}
</style>