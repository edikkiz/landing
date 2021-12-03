<template>
  <div class="row">
    <header>
      <div class="col-3">
        <div v-if="width > 768 || width <= 425" class="logo">
          <img src="../assets/group-2.png" alt="" />
        </div>
        <div v-if="width <= 768 && width > 425" class="logo-tablet">
          <img src="../assets/group-tablet2.png" alt="" />
        </div>
      </div>

      <div class="navbar col-6">
        <div class="navbar-elem">Benefits</div>
        <div class="navbar-elem">Advantages</div>
        <div class="navbar-elem last">Achievements</div>
      </div>

      <div class="col-1"></div>
      <div class="language col-2">
        <div class="language-elem">DE</div>
        <div class="language-elem active">EN</div>
        <div @click="isOpen()" class="burger-menu-icon">
          <img v-if="menuOpen" src="../assets/menu-close.png" />
          <img v-else src="../assets/menu.png" />
        </div>
      </div>
    </header>
  </div>
  <div class="burger-menu" v-if="menuOpen">
    <div class="menu-mobile">
      <div class="title-wrapper">
        <div class="title">Benefits</div>
      </div>
    </div>
    <div class="menu-mobile">
      <div class="title-wrapper">
        <div class="title">Advantages</div>
      </div>
    </div>
    <div class="menu-mobile">
      <div class="title-wrapper">
        <div class="title">Achievements</div>
      </div>
    </div>
    <div class="menu-mobile">
      <div class="title-wrapper">
        <div class="title">Imprint and Data protection</div>
      </div>
    </div>
    <div class="menu-mobile">
      <div class="title-wrapper-language">
        <div class="title-language">Language</div>
        <div class="title-language-elem">DE</div>
        <div class="title-language-elem active">EN</div>
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
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      menuOpen: false,
      width: window.outerWidth,
    };
  },
  methods: {
    isOpen() {
      if (this.menuOpen) {
        this.menuOpen = false;
        document.body.classList.remove("modal-open");
      } else {
        this.menuOpen = true;
        document.body.classList.add("modal-open");
      }
    },
  },
};
</script>

<style lang="scss" scoped>
header {
  .logo {
    margin-left: -95px;
    img {
      cursor: pointer;
    }
  }
  .burger-menu-icon {
    img {
      width: 0;
    }
  }
  height: 144px;
  display: flex;
  align-items: center;
  margin: 0 0 168px;
  .navbar {
    display: flex;
    justify-content: center;
    font-family: $OpenSans;
    font-size: 17px;
    font-weight: 600;
    letter-spacing: 0.13px;
    color: $black;
    text-align: center;
    .navbar-elem {
      cursor: pointer;
      width: 144px;
      height: 23px;
    }
  }
  .language {
    display: flex;
    justify-content: start;
    .language-elem {
      cursor: pointer;
      width: 56px;
      height: 24px;
      opacity: 0.25;
      font-family: $OpenSans;
      font-weight: 600;
      font-size: 17px;
      font-weight: 600;
      letter-spacing: 0.13px;
      color: $black;
      opacity: 0.25;
      text-align: center;
    }
    .active {
      opacity: 1;
    }
  }
}

@media (max-width: 768px) {
  header {
    margin: 0 0 184px 0;
    .logo-tablet {
      margin-left: 66px;
      img {
        cursor: pointer;
      }
    }
    .navbar {
      .navbar-elem {
        width: 120px;
      }
      .last {
        margin-left: 25px;
      }
    }
  }
}
@media (max-width: 426px) {
  header {
    .burger-menu-icon {
      img {
        margin-left: 50px;
        width: 24px;
      }
    }
    .logo {
      margin-left: 37px;
    }
    margin: 0 0 92px;
    .navbar {
      opacity: 0;
      margin-left: -66px;
      .navbar-elem {
        width: 0px;
      }
      .last {
        margin-left: 25px;
      }
    }

    .language {
      display: flex;
      justify-content: start;
      .language-elem {
        opacity: 0;
      }
    }
  }

  .menu-mobile {
    width: 425px;
    padding: 0;
    .title-wrapper-language {
      margin-top: 50px;
      margin-bottom: 50px;
      padding-left: 30px;
      width: 100%;
      height: 56px;
      display: flex;
      flex-direction: row;
      align-items: center;
      border: solid 1px #f3f3f3;
      .title-language {
        width: 187px;
        height: 34px;
        font-family: $Catamaran;
        font-size: 21px;
        font-weight: bold;
        font-stretch: normal;
        font-style: normal;
        line-height: normal;
        letter-spacing: -0.53px;
        color: $black;
      }
      .title-language-elem {
        width: 56px;
        height: 24px;
        opacity: 0.25;
        font-family: $OpenSans;
        font-size: 17px;
        font-weight: 600;
        font-stretch: normal;
        font-style: normal;
        line-height: normal;
        letter-spacing: 0.13px;
        text-align: center;
        color: $black;
      }
      .active {
        opacity: 1;
      }
    }
    .title-wrapper {
      z-index: 2;
      cursor: pointer;
      padding-left: 30px;
      width: 100%;
      height: 56px;
      display: flex;
      flex-direction: row;
      align-items: center;
      border: solid 1px #f3f3f3;
      .title {
        width: 316px;
        height: 34px;
        font-family: $Catamaran;
        font-size: 21px;
        font-weight: bold;
        font-stretch: normal;
        font-style: normal;
        line-height: normal;
        letter-spacing: -0.53px;
        color: $black;
      }
    }
  }

  .burger-menu {
    .button-desk-shadow {
      margin-bottom: 300px;
      box-shadow: 0px 5px 10px 0px rgba(8, 61, 119, 0.5);
      height: 44px;
      .button-desk {
        height: 44px;
      }
    }
    margin-top: -92px;
  }
}
</style>