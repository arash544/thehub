<template>
  <div class="cart">
    <div class="cart-title">
      <img :src="img" alt />
    </div>
    <div class="cart-body">
      <a class="btn-body" href="/">
        <h4>{{txt}}</h4>
        <p>{{desc}}</p>
      </a>
    </div>
    <div class="cart-footer">
      <h5>{{category}}</h5>
      <a v-if="hasbtn" class="btn-footer" href="/">{{btn}}</a>
    </div>
  </div>
</template>


<script>
export default {
  name: "Startupcard",
  props: ["txt", "img", "btn", "category", "desc", "hasbtn"]
};
</script>

<style lang="scss" scoped>

.btn-cart {
  margin-top: -120px;
  width: 100%;
  @media only screen and (min-width: 1000px) {
    margin-top: -70px;
  }
}
.cart {
  width: 350px;
  height: auto;
  margin: 20px;
  padding: 10px;
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
  }
  @media only screen and (min-width: 1000px) {
    margin: 10px 95px;
  }
}
.cart-title {
  display: flex;

  @media only screen and (max-width: 768px) {
    justify-content: center;
    align-items: center;
  }
}
.cart-body {
  @media only screen and (max-width: 768px) {
    text-align: center;
  }
}

.cart-footer {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}
h5 {
  margin-top: 10px;
}
img {
  width: 8vw;
  @media only screen and (max-width: 768px) {
    width: 15vw;
    margin-top: 10px;
  }
}
h4 {
  font-weight: 700;
  margin-top: 20px;
  color: black;
}
p {
  color: rgb(109, 106, 106);
  line-height: 1.3;
  font-weight: 400;
}
.btn-footer,
.btn-body {
  text-decoration: none;
}
.btn-footer {
  background-color: rgb(223, 217, 217);
  color: #4440db;
  font-weight: 700;
  font-size: 18px;
  border: none;
  padding: 5px 10px;
  text-align: center;
}
</style>