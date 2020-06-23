<template>
  <header>
    <nav class="navbar navbar-light bg-light navbar-expand-sm">
      <a class="navbar-brand nav-logo" href="#">
        <img src="https://thehub.io/_nuxt/img/173d5ae.png" alt="logo" />
      </a>
      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#navbar-list-2"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbar-list-2">
        <ul class="navbar-nav ml-auto">
          <li>
            <a class="nav-link" href="#">
              Find jobs
              <span class="sr-only">(current)</span>
            </a>
          </li>
          <li>
            <a class="nav-link" href="#">Browse startups</a>
          </li>
          <li class="spacer"></li>
          <li>
            <a class="nav-link" href="#">For investors</a>
          </li>
          <li>
            <a class="nav-link" href="#">For startups</a>
          </li>
          <li class="spacer"></li>
          <li>
            <a class="nav-link" href="#">Sign up</a>
          </li>
          <li>
            <a class="nav-link" href="#">Log in</a>
          </li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Navbar"
};
</script>

<style lang="scss" scoped>
ul {
  margin-right: 100px;
  @media only screen and (max-width: 768px) {
    display: flex;
    text-align: center;
    justify-content: center;
    margin-right: 0;
  }
}
a {
  font-size: 16px;
  font-weight: 700;
  margin: 5px;
  @media only screen and (max-width: 768px) {
    margin: 0;
  }
}
.spacer {
  height: 30px;
  margin-top: 15px;
  border-left: 1px solid rgba(31, 36, 48, 0.2);
  @media only screen and (max-width: 768px) {
    display: none;
  }
}
img {
  width: 80px;
  height: 50px;
  margin-left: 50px;
}
</style>