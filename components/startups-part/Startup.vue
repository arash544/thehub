<template>
  <div class="wrapper">
    <Startupcard
      img="https://thehub-io.imgix.net/files/s3/20200605090448-79ba86e653779b6f21b91a240122adfc.jpg?fit=crop&w=300&h=300&q=60"
      txt="Momio"
      desc="Momio ApS is an international interactive media company located in Copenhagen, Denmark. The company specializes in developing and operating social online ..."
      category="Education, Gaming"
      btn="2 Jobs"
      hasbtn="true"
    />
    <Startupcard
      img="https://thehub-io.imgix.net/files/s3/20200602132926-c9f6d63627485a27892c01c01dae668a.png?fit=crop&w=300&h=300&q=60"
      txt="Mostly Code"
      desc="Do you dream of becoming part of an innovative web agency focused on sustainable solutions? Mostly Code is a new web agency with many years of experience i..."
      category="SaaS"
      btn="1 Job"
      hasbtn="true"
    />
    <Startupcard
      img="https://thehub-io.imgix.net/files/s3/20200602111406-0547f101bf0fab1728f7a6bcd3111fe9.png?fit=crop&w=300&h=300&q=60"
      txt="Adsensus Denmark"
      desc="We are Adsensus: sales excellence-geeks with a passion for driving and developing the sales process. We have active projects in the Sweden, Norway, Finland and Denmark. Our..."
      category="IT & Software, Advertis..."
      btn="2 Jobs"
      hasbtn="true"
    />
    <Startupcard
      img="https://thehub-io.imgix.net/files/s3/20200514094610-d5fd19e03e57eee21ac933699bc0d915.png?fit=crop&w=300&h=300&q=60"
      txt="Geniale Gaver"
      desc="Genialegaver.dk is a big giftguide, where you can find inspiration and giftideas to find the perfect gift. You can find gifts in easy to navigate categories. Some of the categories..."
      category="Marketplace & eCommerce"
    />
    <Startupcard
      img="https://thehub-io.imgix.net/files/s3/20200511193104-35d22d28d43bb63355d59ad5d84a607f.png?fit=crop&w=300&h=300&q=60"
      txt="Parkbird ApS"
      desc="Parkbird is a parking space company for trucks according to sharing economy principles. We partner up with builders merchant stores, therefore we keep our prices..."
      category="IT & Software, Service"
      btn="2 Jobs"
      hasbtn="true"
    />
    <Startupcard
      img="https://thehub-io.imgix.net/files/s3/20200522120101-360e711f2decb7632b0fb624ca7ef80c.png?fit=crop&w=300&h=300&q=60"
      txt="FieldWorks ApS"
      desc="We aim to create the most user friendly and efficient digital platforms for manual industries. By focusing on great user experience, automation and integration with..."
      category="IT & Software, SaaS, Agr..."
      btn="1 Job"
      hasbtn="true"
    />
      <Categoryimg class="img-startup" img="https://thehub.io/_nuxt/06774af8de756e1a917ebb0036d8504e.svg" />
   
    <Jobsbutton btn="Show All Strtups" />
  </div>
</template>

<script>
import Jobsbutton from "@/components/job-offers/Jobsbutton";
import Categoryimg from "@/components/category-part/Categoryimg";
import Startupcard from "./Startupcard";
export default {
  name: "Startup",
  components: {
    Startupcard,
    Jobsbutton,
    Categoryimg
  }
};
</script>

<style lang="scss" scoped>
.wrapper {
  margin-top: 100px;
  width: 100%;
  display: flex;
  justify-content: space-evenly;
  flex-wrap: wrap;
  @media only screen and (min-width: 1000px) {
    justify-content: center;
  }
}
</style>