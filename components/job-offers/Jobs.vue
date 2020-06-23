<template>
  <div class="main">
    <div class="wrapper">
      <Jobscart
        color="purple"
        title="Other"
        body="Videographer"
        city="Copenhagen"
        situation="Full-time"
        img="https://thehub-io.imgix.net/files/591f0e3ad3ec4cd6659c4e6f/logo_upload-7c421730da5e6831f59a3e8377dc3a8c.png?fit=crop&w=300&h=300&q=60"
        footer="Son of a Tailor"
      />
      <Jobscart
        color="yellow"
        title="Marketing & Communication"
        body="CMO - Partner & Co-founder, Sales & Marketing"
        city="Copenhagen"
        situation="Full-time"
        img="https://thehub-io.imgix.net/files/s3/20200422113236-a88f3ab238f93a86902f701455ec6b59.png?fit=crop&w=300&h=300&q=60"
        footer="Klimate"
      />
      <Jobscart
        color="red"
        title="Design"
        body="Design and User Experience Intern"
        city="Copenhagen"
        situation="Student"
        img="https://thehub-io.imgix.net/files/s3/20190930121047-8701332caafb2f914abf1b06ea5ac54d.png?fit=crop&w=300&h=300&q=60"
        footer="Turis"
      />
      <Jobscart
        color="green"
        title="Marketing & Communication"
        body="Marketing intern"
        city="Denmark"
        situation="Internship"
        img="https://thehub-io.imgix.net/files/59410a86d97bdc195562c4c1/logo_upload-f13bcc8042cd00ed85c030d103a15e74.png?fit=crop&w=300&h=300&q=60"
        footer="GameScorekeeper"
      />
      <Jobscart
        color="purple"
        title="Design"
        body="Visual design student"
        city="Hellerup"
        situation="Part-time"
        img="https://thehub-io.imgix.net/files/s3/20190919112537-70c9230fd5e2f79fc624901fcd47cd0c.png?fit=crop&w=300&h=300&q=60"
        footer="Swiipe Payments"
      />
      <Jobscart
        color="orange"
        title="Marketing & Communication"
        body="Marketing and SEO Assistant"
        city="Copenhagen"
        situation="Internship"
        img="https://thehub-io.imgix.net/files/s3/20191011132136-813eec46e5d6f640a2d04d6f363e831b.png?fit=crop&w=300&h=300&q=60"
        footer="Valuer.ai"
      />
      <Jobsbutton btn="Show All Jobs" />
      <Jobsimg />
    </div>
  </div>
</template>

<script>
import Jobscart from "./Jobscart";
import Jobsbutton from "./Jobsbutton";
import Jobsimg from "./Jobsimg";
export default {
  name: "Jobs",
  components: {
    Jobscart,
    Jobsbutton,
    Jobsimg
  }
};
</script>

<style lang="scss" scoped>
.main {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  width: 100%;
}

.wrapper {
  width: 80%;
  height: auto;
  display: flex;
  margin-top: 100px;
  justify-content: space-around;
  align-items: center;
  flex-wrap: wrap;
  @media only screen and (max-width: 768px) {
    width: 100%;
  }
}
</style>