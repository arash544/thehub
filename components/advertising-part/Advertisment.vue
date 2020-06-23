<template>
  <div class="wrapper">
    <Advertising
      txt="Startups we helped grow"
      img="https://thehub.io/_nuxt/img/60a66f8.png"
      hastxt="true"
    />
    <Advertising img="https://thehub.io/_nuxt/img/95120f8.png" />
    <Advertising img="https://thehub.io/_nuxt/img/e27771a.png" />
    <Advertising img="https://thehub.io/_nuxt/img/189530a.png" />
    <Advertising img="https://thehub.io/_nuxt/img/cb70062.png" />
    <Advertising img="https://thehub.io/_nuxt/img/4ff6907.png" />
  </div>
</template>

<script>
import Advertising from "./Advertising";
export default {
  name: "Advertisment",
  components: {
    Advertising
  }
};
</script>

<style lang="scss" scoped>
.wrapper {
  margin-top: 100px;
  width: 100%;
  padding-right: 30px;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  flex-direction: row;
  flex-wrap: wrap;
  @media only screen and (max-width: 768px) {
    margin-top: 180px;
    padding-right: 0px;
    justify-content: center;
  }
  @media only screen and (max-width: 530px) {
    margin-top: 350px;
  }
}
</style>