<template>
  <section class="main-wrapper">
    <Headertext txt="Find the most exciting startup jobs" />
    <Banner />
    <Advertisment />
    <Headertext txt="Explore by category" />
    <Category />
    <Headertext
      txt="Jobs"
      desctxt="Find a job you love."
      desclink="Go to job search"
      hasdesc="true"
    />
    <Jobs />
    <Headertext
      txt="Startups"
      desctxt="Find your second home."
      desclink="Browse for startups"
      hasdesc="true"
    />
    <Startup />
  </section>
</template>

<script>
import Headertext from "@/components/Headertext";
import Banner from "@/components/Banner-part/Banner";
import Advertisment from "@/components/Advertising-part/Advertisment";
import Category from "@/components/category-part/Category";
import Jobs from "@/components/job-offers/Jobs";
import Startup from "@/components/startups-part/Startup";
export default {
  components: {
    Headertext,
    Banner,
    Advertisment,
    Category,
    Jobs,
    Startup
  }
};
</script>

<style lang="scss" scoped>
.main-wrapper {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  @media only screen and (max-width: 768px) {
    width: 100%;
    display: flex;
    flex-wrap: wrap;
  }
}
</style>