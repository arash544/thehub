<template>
  <div class="cart-content">
    <a href="/">
      <img :src="img" alt />
    </a>
    <h5>{{txt}}</h5>
  </div>
</template>

<script>
export default {
  name: "Categories",
  props: ["txt", "img"]
};
</script>

<style lang="scss" scoped>
.cart-content {
  width: 17%;
  height: 200px;
  padding: 20px 5px;
  background-color: white;
  transition: all 0.5s ease-in-out;
  transition-delay: 0s;
  position: relative;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  padding-right: 40px;
  padding-left: 15px;
  margin: 5px;
  &:hover {
    cursor: pointer;
    transform: translate(0, -10px);
    box-shadow: 0px 10px 35px rgb(183, 231, 243);
  }
  @media only screen and (max-width: 768px) {
    width: 100%;
    margin-top: 15px;
  }
  @media only screen and (min-width: 1000px) {
  }
}
a {
  text-decoration: none;
  @media only screen and (max-width: 768px) {
    margin-top: 10px;
  }
}
h5 {
  margin-top: 20px;
}
img {
  @media only screen and (max-width: 768px) {
    width: 12vw;
    margin-top: 10px;
  }
}
</style>