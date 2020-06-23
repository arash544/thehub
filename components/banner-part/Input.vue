<template>
  <div class="wrapper">
    <form>
      <img src="search.svg" alt />
      <input type="text" placeholder="Job title or keyword" />
      <img src="location.svg" alt />
      <input type="text" placeholder="City or area" />
      <div class="btn-group">
        <button
          type="button"
          class="btn btn-link drop dropdown-toggle"
          data-toggle="dropdown"
          aria-haspopup="true"
          aria-expanded="false"
        >DK</button>
        <div class="dropdown-menu">
          <a class="dropdown-item" href="#">Denmark</a>
          <a class="dropdown-item" href="#">Finland</a>
          <a class="dropdown-item" href="#">Northern Ireland</a>
          <a class="dropdown-item" href="#">Norway</a>
          <a class="dropdown-item" href="#">Sweden</a>
        </div>
      </div>
      <button class="btn btn-lg btn-default">Search</button>
    </form>
  </div>
</template>

<script>
export default {
  name: "Input"
};
</script>

<style lang="scss" scoped>
.wrapper {
  width: 85%;
  height: 100px;
  display: flex;
  background-color: white;
  margin-top: -30px;
  align-items: center;
  position: relative;
  @media only screen and (max-width: 768px) {
    width: 100%;
  }
}
img {
  @media only screen and (max-width: 768px) {
    display: none;
  }
}
form {
  display: flex;
  padding: 5px;
  width: 100%;
  @media only screen and (max-width: 768px) {
    width: 100%;
    flex-direction: column;
  }
}
input {
  padding: 15px;
  width: 30%;
  border: 1px solid white;
  @media only screen and (max-width: 768px) {
    width: 100%;
    margin-top: 5px;
    margin-bottom: 5px;
    border: 1px solid black;
  }
}
.drop {
  padding: 12px;
  @media only screen and (max-width: 768px) {
    margin: 5px;
    width: 100%;
    border: 1px solid black;
  }
}
.btn-default {
  background-color: #4440db;
  padding: 30px 65px;
  color: white;
  border-radius: 0;
  margin-left: 100px;
  @media only screen and (max-width: 768px) {
    padding: 15px 40px;
    width: 100%;
    margin-left: 0;
  }
}
</style>