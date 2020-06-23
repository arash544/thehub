<template>
  <div class="wrapper">
    <h1>{{txt}}</h1>
    <div v-if="hasdesc" class="description">
      <p>{{desctxt}}</p>
      <a href="/">{{desclink}}</a>
    </div>
  </div>
</template>

<script>
export default {
  props: ["txt", "desctxt", "desclink", "hasdesc"]
};
</script>

<style lang="scss" scoped>
h1 {
  font-weight: 700;
  font-size: 60px;
  width: 100%;
}
.wrapper {
  margin-top: 150px;
  width: 33%;
  display: flex;
  flex-direction: column;
  padding-left: 50px;
  align-items: center;
  @media only screen and (max-width: 768px) {
    width: 100%;
    text-align: center;
    padding: 10px;
    margin-left: 0;
  }
}
a {
  margin-left: 5px;
}
a::after {
  content: url("data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTEiIGhlaWdodD0iOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cGF0aCBkPSJNMTAuNzggMy4zOTZMNy42OTMuMjVhLjg0My44NDMgMCAwIDAtMS4xOTUgMCAuODg0Ljg4NCAwIDAgMCAwIDEuMjE4bDEuNjM2IDEuNjdILjg0N0EuODYuODYgMCAwIDAgMCA0YS44Ni44NiAwIDAgMCAuODQ3Ljg2NGg3LjI5OUw2LjQ5OCA2LjUzM2EuODg0Ljg4NCAwIDAgMCAwIDEuMjE4QS44MzYuODM2IDAgMCAwIDcuMDkgOGMuMjIgMCAuNDI5LS4wODMuNTkxLS4yNDlsMy4wNzUtMy4xMzZBLjg1Ljg1IDAgMCAwIDExIDQuMDEyYzAtLjIyNS0uMDctLjQ2Mi0uMjItLjYxNnoiIGZpbGw9IiMzNjg1RDYiIGZpbGwtcnVsZT0ibm9uemVybyIvPjwvc3ZnPg==");
  padding-left: 5px;
}
.description {
  flex-direction: row;
  display: flex;
  width: 100%;
  @media only screen and (max-width: 768px) {
    width: 100%;
    text-align: center;
    justify-content: center;
  }
}
</style>