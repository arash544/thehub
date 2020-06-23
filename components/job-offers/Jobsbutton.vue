<template>
  <div class="wrapper">
    <button>{{btn}}</button>
  </div>
</template>

<script>
export default {
  name: "Jobsbutton",
  props: ["btn"]
};
</script>

<style lang="scss" scoped>
.wrapper {
  width: 100%;
  display: flex;
  justify-content: center;
  margin-top: 100px;
  @media only screen and (max-width: 768px) {
    width: 100%;
  }
}
button {
  padding: 20px 65px;
  font-weight: 600;
  color: white;
  background-color: #4440db;
  border: none;
  @media only screen and (max-width: 768px) {
    width: 80%;
  }
}
</style>