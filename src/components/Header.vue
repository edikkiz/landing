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
