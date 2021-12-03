<template>
  <div class="modal-wrapper">
    <div class="modal">
      <div @click="close" class="modal-close">
        <img src="../assets/img/close-form-button.png" />
      </div>
      <div class="title">
        LET’S DISCUSS <br />
        YOUR BUSINESS CASE!
      </div>
      <div v-if="width > 425" class="text">
        Everything is possible! We will analyze your existing situation,
        discover the bottlenecks and offer a solution that exactly matches your
        business case!
      </div>
      <div v-else class="text">Everything is possible!</div>
      <div class="inputs">
        <div class="input-name">
          <label>First Name</label>
          <input placeholder="Klaus" type="text" />
        </div>
        <div class="input-name">
          <label>Last Name</label>
          <input placeholder="Voormann" type="text" name="" id="" />
        </div>
      </div>
      <div class="inputs">
        <div class="full-wrapper">
          <label>E–Mail</label>
          <input
            class="full"
            placeholder="klaus.voormann@email.de"
            type="text"
          />
        </div>
      </div>
      <div class="inputs">
        <div class="full-wrapper">
          <label>Some brief description or comments</label>
          <textarea
            class="text-box full"
            placeholder="My business case is completely different, so I want to discuss it with you."
          />
        </div>
      </div>
      <div class="privat-text">
        By pressing the “request a consultation” button you agree with
        <a href="https://www.google.com/" target="_blank"
          ><b>data protection</b></a
        >
        policy
      </div>
      <div class="button-modal-wrapper">
        <button @click="close" class="button-modal">
          <div class="button-modal-text">Request a Consultation</div>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Modal",
  methods: {
    close() {
      document.body.classList.remove("modal-open");
      this.$emit("close");
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
.modal-wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
}

.modal {
  box-shadow: 0 10px 30px 0 rgba(30, 30, 30, 0.25);
  -webkit-filter: none;
  filter: none;
  filter: none;
  background-color: white;
  display: flex;
  position: fixed;
  top: 34px;
  flex-direction: column;
  margin: auto;
  width: 633px;
  height: 753px;
  .modal-close {
    cursor: pointer;
    display: flex;
    justify-content: end;
    margin-bottom: 8px;
  }
  .title {
    text-align: start;
    font-family: $Catamaran;
    font-size: 25px;
    font-weight: 900;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.2;
    letter-spacing: -0.63px;
    color: $black;
    margin: 0 0 20px 52px;
  }
  .text {
    width: 529px;
    opacity: 0.75;
    font-family: $OpenSans;
    font-size: 15px;
    font-weight: normal;
    font-stretch: normal;
    font-style: normal;
    line-height: normal;
    letter-spacing: -0.38px;
    color: $black;
    margin: 0 0 50px 52px;
  }
  .inputs {
    display: flex;
    flex-direction: row;
    justify-content: center;
    margin-bottom: 25px;
    font-size: 13px;
    font-family: $OpenSans;
    .input-name {
      margin: 0 12px;
      display: flex;
      flex-direction: column;
      label {
        height: 22px;
      }
      input {
        width: 240px;
        height: 44px;
        object-fit: contain;
        border-radius: 72px;
        border: solid 1px rgba(30, 30, 30, 0.25);
        padding: 10px 22px 10px 24px;
      }
      input::placeholder {
        opacity: 0.25;
      }
    }
    .full-wrapper {
      display: flex;
      flex-direction: column;
      label {
        height: 22px;
      }
      .full {
        width: 504px;
        height: 44px;
        padding: 10px 48.9px 10px 24px;
        object-fit: contain;
        border-radius: 72px;
        border: solid 1px rgba(30, 30, 30, 0.25);
      }
      .full::placeholder {
        opacity: 0.25;
      }
      .text-box {
        font-family: $OpenSans;
        font-size: 17px;
        font-weight: normal;
        font-stretch: normal;
        font-style: normal;
        line-height: normal;
        letter-spacing: -0.43px;
        color: $black;
        height: 132px;
        border-radius: 22px;
        resize: none;
        overflow: auto;
        overflow-x: hidden;
      }
      .text-box::-webkit-scrollbar-thumb {
        background-color: #bbb;
        box-shadow: 0 2px 4px 0 rgba(0, 0, 0, 0.15);
        border-radius: 22px;
        scroll-margin-block-start: 10px;
      }
      .text-box::-webkit-scrollbar {
        border-radius: 22px;
        scroll-margin-block-start: 10px;
      }
    }
    label {
      padding-left: 24px;
    }
  }
  .privat-text {
    margin-left: 64px;
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
    margin-bottom: 50px;
    a {
      color: $black;
    }
  }
  .button-modal-wrapper {
    margin-left: 64px;
    width: 504px;
    display: flex;
    justify-content: end;
    .button-modal {
      width: 240px;
      height: 44px;
      border: none;
      margin-left: -15px;
      background-color: $twilight-blue;
      border-radius: 72px;
      object-fit: contain;
    }
    .button-modal:hover {
      cursor: pointer;
      background-color: #022041;
      transition: 0.5s;
    }
    .button-modal-text {
      font-family: $OpenSans;
      font-size: 17px;
      font-weight: bold;
      font-stretch: normal;
      font-style: normal;
      line-height: normal;
      letter-spacing: -0.43px;
      text-align: center;
      color: #fff;
    }
  }
}
@media (max-width: 768px) {
  .modal {
    top: 34;
    left: 68px;
    .inputs {
      .input-name input {
        font-size: 17px;
      }
      .full-wrapper .full {
        font-size: 17px;
      }
    }
  }
}

@media (max-width: 426px) {
  .modal {
    width: 345px;
    height: 753px;
    top: 30px;
    left: 15px;
    .title {
      margin-left: 25px;
    }
    .text {
      margin-left: 25px;
      margin-bottom: 20px;
    }
    .privat-text {
      width: 295px;
      margin-left: 25px;
      margin-bottom: 25px;
    }

    .button-modal-wrapper {
      margin-left: 80px;
      width: 240px;
    }
    .inputs {
      display: flex;
      flex-direction: column;
      margin-bottom: 10px;
      .input-name {
        margin-left: 25px;
        input {
          width: 295px;
          font-size: 17px;
        }
      }
      .full-wrapper {
        margin-left: 25px;
        .full {
          width: 295px;
          font-size: 17px;
          padding: 13px 24px;
        }
      }
    }
  }
}
</style>