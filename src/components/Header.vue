<template>
  <div class="row">
    <header>
      <div class="col-3"></div>

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
          <img src="../assets/menu.png" />
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
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      menuOpen: false,
    };
  },
  methods: {
    isOpen() {
      if (this.menuOpen) {
        this.menuOpen = false;
        this.$emit("menuOpen", this.menuOpen);
      } else {
        this.menuOpen = true;
        this.$emit("menuOpen", this.menuOpen);
      }
    },
  },
};
</script>
