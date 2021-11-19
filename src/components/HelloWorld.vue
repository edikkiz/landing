<template>
  <div class="container">
    <Header />
    <logisticsManagement />
    <HowYouExperienced />
    <div class="row">
      <div class="col-2"></div>
      <div class="col-4 text-with-procents">
        Expenses reduction after implementing logistics management software!
      </div>
      <div class="col-4 procents">49,2%</div>
      <div class="col-2"></div>
    </div>
    <HowCanYouBenefit />
    <OurAdventages />
  </div>
  <Footer />
</template>

<script>
import Header from "./Header.vue";
import LogisticsManagement from "./Logistics-management.vue";
import HowYouExperienced from "./How-you-experienced.vue";
import HowCanYouBenefit from "./How-can-you-benefit.vue";
import OurAdventages from "./Our-adventages.vue";
import Footer from "./Footer.vue";

export default {
  name: "HelloWorld",
  components: {
    Header,
    LogisticsManagement,
    HowYouExperienced,
    HowCanYouBenefit,
    OurAdventages,
    Footer,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss"></style>
