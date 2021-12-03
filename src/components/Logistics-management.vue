<template>
  <div class="row">
    <div class="col-1"></div>
    <div class="LOGISTICS-MANAGEMENT col-8">
      LOGISTICS MANAGEMENT SOFTWARE DEVELOPMENT
    </div>
  </div>
  <div class="row">
    <a
      v-if="width > 425"
      @click="scrollMeTo()"
      class="col-1 scroll-for-more-info"
    >
      <div class="image">
        <img src="../assets/img/scroll-down-arrow.png" />
      </div>
      <div class="text">Scroll for more information</div>
    </a>
    <div class="col-1"></div>
    <div class="col-7 LOGISTICS-MANAGEMENT-text">
      We solve transportation and stock management problems for Factories,
      Manufacturers, Carriers, Resellers, E-commerce and even more. Any issue
      can be solved with smart digitalization.
    </div>
  </div>
  <div class="row">
    <div class="col-4"></div>
    <div class="col-4">
      <div class="button-desk-shadow">
        <button class="button-desk">
          <div class="button-desk-text">Request a free consultation</div>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Logistics-management",
  methods: {
    scrollMeTo() {
      window.scrollTo({
        top: 30000,
        behavior: "smooth",
      });
    },
  },
  data() {
    return {
      width: window.outerWidth,
    };
  },
};
</script>

<style lang="scss" scoped>
.LOGISTICS-MANAGEMENT {
  margin: 0 0 49px;
  text-align: start;
  height: 110px;
  font-family: $Catamaran;
  font-size: 55px;
  font-weight: 900;
  line-height: 1;
  letter-spacing: -1.38px;
  color: $black;
}

.LOGISTICS-MANAGEMENT-text {
  width: 566px;
  padding: 0;
  margin: 0 0 62px -40px;
  opacity: 0.75;
  font-family: $OpenSans;
  font-size: 21px;
  font-weight: 400;
  letter-spacing: -0.53px;
  color: $charcoal;
}

.scroll-for-more-info {
  cursor: pointer;
  display: flex;
  flex-direction: row;
  width: 207px;
  height: 36px;
  transform: rotate(-90deg);
  margin-left: -150px;
  opacity: 0.5;
  font-family: $OpenSans;
  font-size: 13px;
  font-weight: 300;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: 0.16px;
  text-align: center;
  color: $charcoal;
  img {
    margin-left: -100px;
    transform: rotate(90deg);
  }
  padding: 0;
}

@media (max-width: 768px) {
  .LOGISTICS-MANAGEMENT {
    padding: 0;
    font-size: 35px;
    width: 452px;
    height: 70px;
    letter-spacing: -0.88px;
    margin-left: 80px;
  }

  .LOGISTICS-MANAGEMENT-text {
    width: 452px;
    font-size: 17px;
    letter-spacing: -0.43px;
    margin: 0 0 87px -82px;
  }

  .scroll-for-more-info {
    margin-top: 20px;
    margin-left: -45px;
  }
}

@media (max-width: 426px) {
  .LOGISTICS-MANAGEMENT {
    padding: 0;
    font-size: 30px;
    width: 325px;
    height: 120px;
    letter-spacing: -0.75px;
    margin-bottom: 50px;
    margin-left: 5px;
  }

  .LOGISTICS-MANAGEMENT-text {
    margin-left: 35px;
    margin-bottom: 50px;
    width: 325px;
    height: 138px;
  }

  .scroll-for-more-info {
    opacity: 0;
  }
}
</style>