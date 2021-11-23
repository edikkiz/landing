<template>
  <div v-bind:class="{ modalContainer: isModalVisible }" @click="isModalOpen()" class="container">
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
    <div class="row">
      <div class="col-4"></div>
      <div class="col-4">
        <div class="button-desk-shadow">
          <button class="button-desk">
            <div @click="openModal(); modalOpen()" class="button-desk-text">
              Fill in the contact form
            </div>
          </button>
        </div>
      </div>
    </div>
    <OurAdventages />
    <Footer />
  </div>
  <Modal v-if="isModalVisible" @close="isModalVisible = false"  />
</template>

<script>
import Header from "./Header.vue";
import LogisticsManagement from "./Logistics-management.vue";
import HowYouExperienced from "./How-you-experienced.vue";
import HowCanYouBenefit from "./How-can-you-benefit.vue";
import OurAdventages from "./Our-adventages.vue";
import Footer from "./Footer.vue";
import Modal from "./Modal.vue";

export default {
  name: "Landing",
  components: {
    Header,
    LogisticsManagement,
    HowYouExperienced,
    HowCanYouBenefit,
    OurAdventages,
    Footer,
    Modal,
  },
  data() {
    return {
      isModalVisible: false,
    };
  },
  methods: {
    modalOpen () {
      document.body.classList.add('modal-open')
      return
    },
    isModalOpen () {
      if (this.isModalVisible) {
      document.body.classList.remove('modal-open')
        this.isModalVisible = false
        return
      }
      else {
        return
      }
    },
    openModal () {
      setTimeout(() => {
        this.isModalVisible = true
        }, 100)
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss"></style>
