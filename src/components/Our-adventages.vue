<template>
  <div class="row our-advantages-block">
    <div class="col-1"></div>
    <div class="col-5">
      <div class="our-advantages">OUR ADVANTAGES</div>
      <div class="our-advantages-notations-wrapper">
        <div class="notation">
          <div class="icon">
            <img src="../assets/img/decorative-red-dot.png" />
          </div>
          <div class="title-text">
            <div class="title">System Integration</div>
            <div class="text">
              We help you with educating employees and integrating software in
              your running processes
            </div>
          </div>
        </div>

        <div class="notation-mobile">
          <div @click="showText(1)" class="title-wrapper">
            <div class="title">System Integration</div>
            <img v-if="notationText1" src="../assets/pin-up.png" />
            <img v-else src="../assets/pin-down.png" />
          </div>
          <div v-if="notationText1" class="text">
            We help you with educating employees and integrating software in
            your running processes
          </div>
        </div>
      </div>
      <div class="our-advantages-notations-wrapper">
        <div class="notation">
          <div class="icon">
            <img src="../assets/img/decorative-red-dot.png" />
          </div>
          <div class="title-text">
            <div class="title">Technical support</div>
            <div class="text">
              We guarantee support and product maintenance after release and
              keep improving the system in cooperation with your team
            </div>
          </div>
        </div>

        <div class="notation-mobile">
          <div @click="showText(2)" class="title-wrapper">
            <div class="title">Technical support</div>
            <img v-if="notationText2" src="../assets/pin-up.png" />
            <img v-else src="../assets/pin-down.png" />
          </div>
          <div v-if="notationText2" class="text">
            We guarantee support and product maintenance after release and keep
            improving the system in cooperation with your team
          </div>
        </div>
      </div>
      <div class="our-advantages-notations-wrapper">
        <div class="notation">
          <div class="icon">
            <img src="../assets/img/decorative-red-dot.png" />
          </div>
          <div class="title-text">
            <div class="title">Data security</div>
            <div class="text">
              Your data is stored on secure servers based in Germany (or any
              other country on your request)
            </div>
          </div>
        </div>

        <div class="notation-mobile">
          <div @click="showText(3)" class="title-wrapper">
            <div class="title">Data security</div>
            <img v-if="notationText3" src="../assets/pin-up.png" />
            <img v-else src="../assets/pin-down.png" />
          </div>
          <div v-if="notationText3" class="text">
            Your data is stored on secure servers based in Germany (or any other
            country on your request)
          </div>
        </div>
      </div>
      <div class="our-advantages-notations-wrapper">
        <div class="notation">
          <div class="icon">
            <img src="../assets/img/decorative-red-dot.png" />
          </div>
          <div class="title-text">
            <div class="title">We speak your language</div>
            <div class="text">
              Our managers are German- and English-speaking, so the business
              communication is clear and easy
            </div>
          </div>
        </div>

        <div class="notation-mobile">
          <div @click="showText(4)" class="title-wrapper">
            <div class="title">We speak your language</div>
            <img v-if="notationText4" src="../assets/pin-up.png" />
            <img v-else src="../assets/pin-down.png" />
          </div>
          <div v-if="notationText4" class="text">
            Our managers are German- and English-speaking, so the business
            communication is clear and easy
          </div>
        </div>
      </div>
      <div class="our-advantages-notations-wrapper">
        <div class="notation">
          <div class="icon">
            <img src="../assets/img/decorative-red-dot.png" />
          </div>
          <div class="title-text">
            <div class="title">Representative in Germany</div>
            <div class="text">
              Our business analyst is based in Frankfurt am Main. Discussing all
              the business issues in person is much more efficient
            </div>
          </div>
        </div>

        <div class="notation-mobile">
          <div @click="showText(5)" class="title-wrapper">
            <div class="title">Representative in Germany</div>
            <img v-if="notationText5" src="../assets/pin-up.png" />
            <img v-else src="../assets/pin-down.png" />
          </div>
          <div v-if="notationText5" class="text">
            Our business analyst is based in Frankfurt am Main. Discussing all
            the business issues in person is much more efficient
          </div>
        </div>
      </div>
      <div class="our-advantages-notations-wrapper">
        <div class="notation">
          <div class="icon">
            <img src="../assets/img/decorative-red-dot.png" />
          </div>
          <div class="title-text">
            <div class="title">5 years experience in logistics</div>
            <div class="text">
              We’ve successfully implemented custom logistics/ <br />
              transportation/stock and order management systems
            </div>
          </div>
        </div>

        <div class="notation-mobile">
          <div @click="showText(6)" class="title-wrapper">
            <div class="title">5 years experience in logistics</div>
            <img v-if="notationText6" src="../assets/pin-up.png" />
            <img v-else src="../assets/pin-down.png" />
          </div>
          <div v-if="notationText6" class="text">
            We’ve successfully implemented custom logistics/ <br />
            transportation/stock and order management systems
          </div>
        </div>
      </div>
    </div>
    <div class="col-1"></div>
    <div class="col-5">
      <div class="our-advantages-person-wrapper">
        <div class="our-advantages-notations-wrapper">
          <div class="person-wrapper">
            <div class="text">
              <b>
                Flawless communication with the Clockwise Software team resulted
                in a fleet management system that exactly met the needs of the
                municipal waste transportation company. The software runs on
                Android smartphones, so there was no need for expensive
                equipment, and the learning curve was low. We’ve implemented
                multi-tenancy to use this software in other projects connected
                with logistics.</b
              >
            </div>
            <div class="icon-title">
              <div class="icon">
                <img src="../assets/img/person-img/Dan-Weber.png" />
              </div>
              <div class="title">
                <b>Dan Weber</b> <br />
                CEO/CTO at Marketsoup
              </div>
            </div>
          </div>
        </div>
        <div class="our-advantages-notations-wrapper">
          <div class="person-wrapper">
            <div class="text">
              <b>
                With the automatic load scheduling and proper route planning, we
                are finally able to use 100% of our truck load capacity. Also,
                order management and delivery have become much more efficient
                due to custom modules. In the first year, we have covered our
                investment in custom ERP system development</b
              >
            </div>
            <div class="icon-title">
              <div class="icon">
                <img src="../assets/img/person-img/Vadim-Chabanenko.png" />
              </div>
              <div class="title">
                <b>Vadim Chabanenko</b> <br />
                Director at UDK Gazbeton
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      notationText1: false,
      notationText2: false,
      notationText3: false,
      notationText4: false,
      notationText5: false,
      notationText6: false,
    };
  },
  methods: {
    showText(number) {
      if (this.notationText1 === false && number === 1) {
        this.notationText1 = true;
        return;
      } else if (this.notationText1 === true && number === 1) {
        this.notationText1 = false;
        return;
      }
      if (this.notationText2 === false && number === 2) {
        this.notationText2 = true;
        return;
      } else if (this.notationText2 === true && number === 2) {
        this.notationText2 = false;
        return;
      }
      if (this.notationText3 === false && number === 3) {
        this.notationText3 = true;
        return;
      } else if (this.notationText3 === true && number === 3) {
        this.notationText3 = false;
        return;
      }
      if (this.notationText4 === false && number === 4) {
        this.notationText4 = true;
        return;
      } else if (this.notationText4 === true && number === 4) {
        this.notationText4 = false;
        return;
      }
      if (this.notationText5 === false && number === 5) {
        this.notationText5 = true;
        return;
      } else if (this.notationText5 === true && number === 5) {
        this.notationText5 = false;
        return;
      }
      if (this.notationText6 === false && number === 6) {
        this.notationText6 = true;
        return;
      } else if (this.notationText6 === true && number === 6) {
        this.notationText6 = false;
        return;
      }
    },
  },
  name: "Our-adventages",
};
</script>

<style lang="scss" scoped>
.our-advantages {
  font-family: $Catamaran;
  font-size: 35px;
  font-weight: 900;
  font-stretch: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: -0.88px;
  color: $black;
  margin-bottom: 52px;
  height: 44px;
  width: 505px;
}

.our-advantages-person-wrapper {
  background-color: #ffffff;
  box-shadow: 0 10px 30px 0 rgba(0, 0, 0, 0.1);
  width: 633px;
  height: 757px;
  padding: 96px 158px 133px 40px;
  margin: 0 0 229px -20px;
}

.our-advantages-block {
  margin-left: 10px;
}

.our-advantages-notations-wrapper {
  margin-right: -20px;
  .notation-mobile {
    font-size: 0;
    img {
      width: 0;
    }
  }
  .notation {
    display: flex;
    .icon {
      margin-right: 43px;
    }
    .title-text {
      .title {
        font-family: $Catamaran;
        font-size: 21px;
        font-weight: 900;
        font-stretch: normal;
        font-style: normal;
        line-height: normal;
        letter-spacing: -0.53px;
        color: $black;
      }
      .text {
        width: $textWidth;
        opacity: 0.75;
        font-family: $OpenSans;
        font-size: 15px;
        font-weight: normal;
        font-stretch: normal;
        font-style: normal;
        line-height: normal;
        letter-spacing: -0.38px;
        color: $black;
        margin-bottom: 26px;
      }
    }
  }
  .person-wrapper {
    .text {
      width: 435px;
      font-family: $OpenSans;
      font-size: 17px;
      font-weight: bold;
      font-stretch: normal;
      font-style: normal;
      line-height: normal;
      letter-spacing: -0.43px;
      color: $black;
      margin-bottom: 15px;
    }
    .icon-title {
      width: 435px;
      display: flex;
      flex-direction: row-reverse;
      .title {
        font-family: $OpenSans;
        font-size: 15px;
        font-weight: normal;
        font-stretch: normal;
        font-style: normal;
        line-height: normal;
        letter-spacing: -0.43px;
        text-align: right;
        color: $black;
      }
      .icon {
        margin: 0 0 71px 15px;
        filter: grayscale(100%);
      }
    }
  }
}

@media (max-width: 768px) {
  .our-advantages-block {
    display: flex;
    flex-direction: column;
    margin-top: 29px;
    .our-advantages {
      font-size: 25px;
    }
  }
  .our-advantages-person-wrapper {
    width: 633px;
    height: 708px;
    padding: 90px 110px 90px 108px;
    margin-left: -11px;
  }
}
@media (max-width: 426px) {
  .our-advantages-notations-wrapper {
    .notation .icon img {
      width: 0;
    }

    .title-wrapper {
      margin-left: 20px;
    }
    .notation .title-text {
      .title {
        font-size: 0;
      }
      .text {
        font-size: 0;
        margin-bottom: 0;
      }
    }
    .notation {
      height: 0;
    }

    .notation-mobile {
      width: 430px;
      padding: 0;
      margin-left: -25px;
      padding-left: 10px;
      border: solid 1px #f3f3f3;
      .title-wrapper {
        z-index: 2;
        cursor: pointer;
        padding-left: 25px;
        width: 100%;
        height: 56px;
        display: flex;
        flex-direction: row;
        align-items: center;
        margin-left: 0;
        .title {
          width: 306px;
          height: 34px;
          font-family: $Catamaran;
          font-size: 21px;
          font-weight: 900;
          font-stretch: normal;
          font-style: normal;
          line-height: normal;
          letter-spacing: -0.53px;
          color: $black;
        }
        img {
          width: 18px;
          height: 10px;
        }
      }
      .text {
        margin-left: 22px;
        padding-left: 15px;
        width: 345px;
        opacity: 0.75;
        font-family: $OpenSans;
        font-size: 15px;
        font-weight: normal;
        font-stretch: normal;
        font-style: normal;
        line-height: normal;
        letter-spacing: -0.38px;
        color: $black;
      }
    }
  }

  .our-advantages {
    width: 345px;
    margin-left: 35px;
  }

  .our-advantages-person-wrapper {
    padding: 25px;
    margin-top: 98px;
    margin-left: 5px;
    width: 345px;
    height: 625px;
    .person-wrapper {
      .text {
        width: 300px;
        margin-bottom: 15px;
        font-size: 15px;
        font-weight: 600;
        letter-spacing: -0.38px;
      }
      .icon-title {
        width: 295px;
        .icon {
          margin-bottom: 50px;
        }
      }
    }
  }
}
</style>