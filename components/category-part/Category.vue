<template>
  <div class="wrapper">
    <div class="cart">
      <Categories
        img="https://thehub.io/_nuxt/45bfb656342e6becfc12dda4af66b074.svg"
        txt="Business Development"
      />
      <Categories
        img="https://thehub.io/_nuxt/136b12838d2cf16bfb0af0b72acc5122.svg"
        txt="Customer Service"
      />
      <Categories img="https://thehub.io/_nuxt/a90c3fcb95a39d140aa2651f20d8ee96.svg" txt="Design" />
      <Categories
        img="https://thehub.io/_nuxt/5098bddab599270aacc209eadf2ed6be.svg"
        txt="Development"
      />
      <Categories
        img="https://thehub.io/_nuxt/373a4d83ef6965acad966489419d3d30.svg"
        txt="Mobile Development"
      />
      <Categories
        img="https://thehub.io/_nuxt/84fadb4ef804a3856faa66df99e69966.svg"
        txt="Business Intelligence"
      />
      <Categories
        img="https://thehub.io/_nuxt/56e3d8125fbc7817f6d37bb0da159c11.svg"
        txt="Marketing & Communication"
      />
      <Categories
        img="https://thehub.io/_nuxt/b258cbe9f2ed91136902a0cb80b79f61.svg"
        txt="Project Management"
      />
      <Categories img="https://thehub.io/_nuxt/3447d583e38368a6cca85921cc955ace.svg" txt="Sales" />
      <Categoryimg class="img-category" img="https://thehub.io/_nuxt/c50e03997229d2ae16222a82f9d2e3be.svg" />
    </div>
  </div>
</template>

<script>
import Categoryimg from "./Categoryimg";
import Categories from "./Categories";
export default {
  name: "Category",
  components: {
    Categoryimg,
    Categories
  }
};
</script>

<style lang="scss" scoped>
.wrapper {
  margin-top: 100px;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
  flex-wrap: wrap;
  height: auto;
  @media only screen and (max-width: 768px) {
    text-align: center;
  }
}
.cart {
  width: 80%;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  flex-direction: row;
  flex-wrap: wrap;
  @media only screen and (max-width: 768px) {
  }
}
</style>