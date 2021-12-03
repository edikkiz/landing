<template>
  <footer>
    <div class="nav-wrapper">
      <div class="nav data-protection">Data Protection</div>
      <div class="nav imprint">Imprint</div>
    </div>
    <div class="nav-wrapper-modile">
      <div class="nav data-protection-mobile">Data Protection / Imprint</div>
    </div>
    <div><img src="../assets/img/image_2021-11-19_14-20-46.png" /></div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style lang="scss" scoped>
footer {
  img {
    cursor: pointer;
  }
  .nav-wrapper-modile {
    .data-protection-mobile {
      font-size: 0;
    }
  }
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-around;
  height: 104px;
  background-color: $black;
  .nav-wrapper {
    display: flex;
    .nav {
      cursor: pointer;
      font-family: $OpenSans;
      font-size: 15px;
      font-weight: 600;
      font-stretch: normal;
      font-style: normal;
      line-height: normal;
      letter-spacing: 0.12px;
      text-align: center;
      color: #fff;
      height: 20px;
      margin-left: 20px;
    }
    .imprint {
      width: 80px;
    }
    .data-protection {
      width: 175px;
    }
  }
}

@media (max-width: 768px) {
  footer {
    img {
      cursor: pointer;
    }
    width: 100%;
    .nav-wrapper-modile {
      .data-protection-mobile {
        cursor: pointer;
        font-family: $OpenSans;
        font-size: 15px;
        font-weight: 600;
        font-stretch: normal;
        font-style: normal;
        line-height: normal;
        letter-spacing: 0.12px;
        text-align: center;
        color: #fff;
        height: 20px;
        margin-left: -500px;
      }
    }
    .nav-wrapper {
      .data-protection,
      .imprint {
        font-size: 0;
      }
    }
  }
}
@media (max-width: 426px) {
  footer {
    img {
      margin-left: -100px;
      cursor: pointer;
    }
    .nav-wrapper {
      .data-protection {
        font-size: 0;
      }
      .imprint {
        font-size: 0;
      }
    }
    .nav-wrapper-modile {
      .data-protection-mobile {
        text {
          cursor: pointer;
        }
        width: 200px;
        height: 20px;
        margin: -20px 0 36px;

        font-family: $OpenSans;
        font-size: 15px;
        font-weight: 600;
        font-stretch: normal;
        font-style: normal;
        line-height: normal;
        letter-spacing: 0.12px;
        text-align: center;
        color: #fff;
      }
    }
    display: flex;
    justify-content: center;
    flex-direction: column;
    margin-left: 0;
    width: 100%;
    height: 208px;
  }
}
</style>