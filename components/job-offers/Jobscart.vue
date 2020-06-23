<template>
  <div class="cart">
    <div class="cart-title">
      <svg class="circle">
        <circle cx="15" cy="15" r="7" :fill="color" stroke-width="1" />
      </svg>
      <h6>{{title}}</h6>
    </div>
    <div class="cart-body">
      <h4>{{body}}</h4>
      <a href="/">{{city}}</a>
      <img class="dot" src="dot.svg" alt />
      <a href="/">{{situation}}</a>
    </div>
    <div class="cart-footer">
      <img class="logo" :src="img" alt />
      <h6 class="logo-txt">
        <b>{{footer}}</b>
      </h6>
    </div>
  </div>
</template>

<script>
export default {
  name: "Jobscart",
  props: [
    "footer",
    "img",
    "logo",
    "body",
    "situation",
    "city",
    "title",
    "circle",
    "color"
  ]
};
</script>

<style lang="scss" scoped>
.cart {
  width: 350px;
  height: 350px;
  margin: 40px;
  background-color: white;
  transition: all 0.5s ease-in-out;
  transition-delay: 0s;
  z-index: 100;
  position: relative;
  &:hover {
    cursor: pointer;
    transform: translate(0, -10px);
    box-shadow: 0px 30px 80px rgb(133, 136, 136);
  }
  @media only screen and (max-width: 768px) {
    width: 100%;
    margin-top: 20px;
    height: auto;
    padding: 10px;
  }
}
h4 {
  padding-left: 5px;
}
h6 {
  margin-left: 10px;
  margin-top: 5px;
  @media only screen and (max-width: 768px) {
    font-size: 18px;
  }
}
.cart-title {
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: center;
  padding-left: 10px;
  @media only screen and (max-width: 768px) {
    justify-content: center;
    width: 100%;
    font-size: 28px;
  }
}
.cart-body {
  padding-left: 10px;
  margin-top: 10px;
  @media only screen and (max-width: 768px) {
    text-align: center;
  }
  a {
    margin: 5px;
  }
}

.cart-footer {
  padding-left: 10px;
  display: flex;
  margin-top: 70px;
  align-items: center;
  @media only screen and (max-width: 768px) {
    justify-content: center;
    align-items: center;
  }
  @media only screen and (max-width: 420px) {
    justify-content: center;
  }
}
.circle {
  width: 30px;
  height: 30px;
  @media only screen and (max-width: 768px) {
    width: 10vw;
    text-align: center;
  }
}
.dot {
  width: 0.6vw;
  @media only screen and (max-width: 768px) {
    width: 2vw;
  }
}
.logo {
  max-width: 4vw;
  @media only screen and (max-width: 768px) {
    max-width: 10vw;
  }
}
.logo-txt {
  padding-top: 10px;
  @media only screen and (max-width: 768px) {
    padding-top: 0px;
    font-size: 20px;
  }
}
a {
  color: gray;
}
</style>
  
    