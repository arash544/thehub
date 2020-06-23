<template>
  <ul>
    <li v-if="hastxt">
      <h5>{{txt}}</h5>
    </li>
    <li>
      <img :src="img" alt />
    </li>
  </ul>
</template>

<script>
export default {
  name: "Advertising",
  props: ["txt", "img", "hastxt"]
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
  @media only screen and (max-width: 768px) {
    margin-top: 180px;
    padding-right: 0px;
    justify-content: center;
  }
  @media only screen and (max-width: 530px) {
    margin-top: 350px;
  }
}
ul {
  display: flex;
  justify-content: flex-end;
  flex-direction: row;
  align-items: center;
  flex-wrap: wrap;
  @media only screen and (max-width: 768px) {
    width: 100%;
    margin-top: 0;
    padding-left: 0;
    justify-content: center;
  }
}
img {
  max-width: 7vw;
  @media only screen and (max-width: 768px) {
    width: 30vw;
    max-width: 20vw;
  }
}

h5 {
  font-weight: 300;
  @media only screen and (max-width: 768px) {
    font-size: 30px;
  }
}
li {
  list-style-type: none;
  margin: 0 15px;
  @media only screen and (max-width: 768px) {
    margin: 15px 0 0 0;
    width: 100%;
    justify-content: center;
    display: flex;
    align-items: center;
  }
}
</style>