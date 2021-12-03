<template>
  <div class="row">
    <div class="col-1"></div>
    <div class="col-10 title Have-you-experienced">
      HAVE YOU EXPERIENCED ANY OF THESE ISSUES?
    </div>
  </div>

  <Carousel class="carousel" />
</template>

<script>
import Carousel from "./Carousel.vue";

export default {
  components: { Carousel },
  name: "How-you-experienced",
};
</script>

<style lang="scss" scoped>
.Have-you-experienced {
  margin: 0 0 168px;
  font-size: 35px;
  font-family: $Catamaran;
  font-weight: 900;
  line-height: 1;
  letter-spacing: -0.88px;
  text-align: right;
  height: 35px;
  color: $black;
}

@media (max-width: 768px) {
  .Have-you-experienced {
    height: 25px;
    margin-left: 35px;
    width: 585px;
    font-size: 25px;
  }
}

@media (max-width: 426px) {
  .Have-you-experienced {
    width: 345px;
    height: 50px;
    letter-spacing: -0.63px;
    margin-left: 20px;
    padding: 0;
    margin-bottom: 50px;
  }
}
</style>