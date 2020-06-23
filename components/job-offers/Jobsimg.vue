<template>
  <div class="wrapper">
    <img src="https://thehub.io/_nuxt/8afe9ec4cbffc97a1c39468a2f9a880f.svg" alt />
  </div>
</template>

<script>
export default {
  name: "Jobsimg"
};
</script>

<style lang="scss" scoped>
.wrapper {
  position: relative;
}
img {
  width: 22vw;
  position: absolute;
  bottom: 100px;
  right: -50px;
  z-index: -10;
  @media only screen and (max-width: 1100px) {
    display: none;
  }
}
</style> 