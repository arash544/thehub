<template>
  <div class="wrapper">
    <div class="footer">
      <div class="footer-header">
        <p>The Hub is active in :</p>
      </div>
      <div class="footer-body">
        <h3>Denmark</h3>
        <h3>Finland</h3>
        <h3>Northern Ireland</h3>
        <h3>Norway</h3>
        <h3>Sweden</h3>
      </div>
      <div class="footer-footer">
        <img src="hub.ico" alt />
        <a href="/">About</a>
        <a href="/">Privacy</a>
        <a href="/">Terms</a>
        <a href="/">Tools</a>
        <a href="/">Partners</a>
        <a href="/">Contact</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footers"
};
</script>

<style lang="scss" scoped>
.wrapper {
  margin-top: 100px;
  width: 100%;
  background-color: #1f2430;
  right: 0;
  left: 0;
  bottom: 0;
  width: 100%;
  height: 500px;
  display: flex;
  flex-direction: column;
  margin-top: 100px;
  flex-wrap: wrap;
  @media only screen and (max-width: 768px) {
    height: auto;
  }
}
.footer {
  padding: 100px 55px;
  width: 100%;
  height: 500px;
  @media only screen and (max-width: 768px) {
    height: auto;
  }
}
p {
  color: #c2e0e8;
  font-size: 26px;
  @media only screen and (max-width: 768px) {
    text-align: center;
  }
}
a {
  color: white;
}
img {
  background-color: white;
  color: white;
  border: 0;
}
.footer-body {
  color: #5aeadc;
  font-size: 23px;
  display: flex;
  flex-wrap: wrap;
}
h3,
p,
img,
a {
  margin: 10px;
}
.footer-body,
.footer-header,
.footer-footer {
  margin-top: 30px;
  padding: 10px;
}
.footer-footer {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
}
.footer-header {
  display: flex;
  flex-direction: row;
  justify-content: center;
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  p {
    width: 100%;
    flex-direction: row;
    justify-content: center;
  }
}
</style>