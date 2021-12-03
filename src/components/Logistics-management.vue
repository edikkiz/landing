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
