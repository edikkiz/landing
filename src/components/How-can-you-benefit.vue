<template>
  <div class="row">
    <div class="col-1"></div>
    <div class="col-7 HOW-CAN-YOU-BENEFIT">
      HOW CAN YOU BENEFIT FROM <br />
      CUSTOM LOGISTICS SOFTWARE?
      <div class="HOW-CAN-YOU-BENEFIT-mobile">
        LOGISTICS MANAGEMENT SOFTWARE DEVELOPMENT
      </div>
    </div>
  </div>
  <div class="row notation-row">
    <div class="col-6 notation-block">
      <div class="notation-wrapper">
        <div class="notation-icone">
          <img src="../assets/img/notation/group-1.png" />
        </div>
        <div>
          <div class="notation-title">Customized to your needs</div>
          <div class="notation-text">
            A software is developed exclusively with your needs and plans in
            mind. This enables to solve unique problems efficiently
          </div>
        </div>
      </div>
    </div>
    <div class="col-6 notation-block right">
      <div class="notation-wrapper">
        <div class="notation-icone">
          <img src="../assets/img/notation/group-2.png" />
        </div>
        <div>
          <div class="notation-title">Short-term ROI</div>
          <div class="notation-text">
            You will experience the first returns right in the first month after
            integrating the system in your current processes
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="row notation-row">
    <div class="col-6 notation-block">
      <div class="notation-wrapper">
        <div class="notation-icone">
          <img src="../assets/img/notation/group-3.png" />
        </div>
        <div>
          <div class="notation-title">Predictable scalability</div>
          <div class="notation-text">
            A custom system grows along with your business since your company
            goals are taken into account in the development process
          </div>
        </div>
      </div>
    </div>
    <div class="col-6 notation-block right">
      <div class="notation-wrapper">
        <div class="notation-icone">
          <img src="../assets/img/notation/group-4.png" />
        </div>
        <div>
          <div class="notation-title">Improve, not rebuild</div>
          <div class="notation-text">
            Custom software supports and improves your running processes
            step-by-step. Your current system keeps working
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="row">
    <div class="col-4"></div>
    <div class="col-4 YOUR-BUSINESS-CASE">
      YOUR BUSINESS CASE <br />
      IS COMPLETELY DIFFERENT?
      <p>LET’S DISCUSS</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "How-can-you-benefit",
  methods: {
    close() {
      this.$emit("close");
    },
  },
};
</script>

<style lang="scss" scoped>
.YOUR-BUSINESS-CASE {
  width: 355px;
  font-family: $Catamaran;
  font-size: 25px;
  font-weight: 900;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.2;
  letter-spacing: -0.63px;
  text-align: center;
  color: $black;
  margin-bottom: 30px;
  margin-left: 25px;
  p {
    margin-top: 0;
    margin-bottom: 0;
    color: $watermelon;
  }
}

.HOW-CAN-YOU-BENEFIT {
  width: 710px;
  height: 70px;
  margin: 0 0 127px 54px;
  font-family: $Catamaran;
  font-size: 35px;
  font-weight: 900;
  font-stretch: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: -0.88px;
  color: $black;
  .HOW-CAN-YOU-BENEFIT-mobile {
    margin-left: 15px;
    font-size: 0;
  }
}

.our-advantages-notations-wrapper {
  .notation-mobile {
    font-size: 0;
    img {
      width: 0;
    }
  }
}

.notation-block {
  padding-left: 80px;
  .notation-wrapper {
    display: flex;
    .notation-icone {
      padding: 15px 23px 0 0;
    }
    .notation-text {
      width: $textWidth + 1;
      color: $black;
      font-family: $OpenSans;
      font-size: 17px;
      font-weight: 400;
      font-stretch: normal;
      font-style: normal;
      line-height: normal;
      letter-spacing: -0.43px;
      margin-bottom: 47px;
    }
    .notation-title {
      font-family: $Catamaran;
      font-size: 25px;
      font-weight: 900;
      font-stretch: normal;
      font-style: normal;
      line-height: normal;
      letter-spacing: -0.63px;
      text-align: start;
      color: $black;
      margin-bottom: 20px;
    }
  }
  .right {
    padding-left: 47px;
  }
}

@media (max-width: 768px) {

  .YOUR-BUSINESS-CASE {
    margin-top: 157px;
    margin-left: -45px;
  }
  .HOW-CAN-YOU-BENEFIT {
    padding: 0;
    padding-left: 48px;
    font-size: 25px;
    margin-bottom: 121px;
  }
  .notation-row {
    display: flex;
    flex-direction: column;
  }

  .notation-block {
    padding-left: 0;
    margin-left: 58px;
    .notation-wrapper {
      .notation-text {
        font-weight: normal;
      }
      .notation-title {
        font-size: 21px;
        letter-spacing: -0.53px;
      }
    }
  }
}

@media (max-width: 426px) {
  .YOUR-BUSINESS-CASE {
    margin-top: 118px;
    letter-spacing: -0.53px;
    line-height: 1.19;
    font-size: 21px;
    margin-left: 25px;
  }
  .HOW-CAN-YOU-BENEFIT {
    font-size: 0;
    margin-left: 15px;
    .HOW-CAN-YOU-BENEFIT-mobile {
      margin-left: -35px;
      width: 345px;
      height: 50px;
      font-family: $Catamaran;
      font-size: 25px;
      font-weight: 900;
      font-stretch: normal;
      font-style: normal;
      line-height: 1;
      letter-spacing: -0.63px;
      color: $black;
    }
  }
  .notation-block {
    margin-left: 0;
    .notation-wrapper {
      .notation-title {
        width: 220px;
        line-height: 1;
        text-transform: uppercase;
        margin-bottom: 10px;
      }
      .notation-text {
        width: 220px;
        font-size: 15px;
        letter-spacing: -0.38px;
        opacity: 0.75;
        margin-bottom: 44px;
      }
    }
  }
}
</style>