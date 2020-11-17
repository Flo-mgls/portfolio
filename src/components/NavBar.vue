<template>
  <nav class="navbar navbar-expand-md fixed-top py-0" :class="nav">
    <div class="navbar-collapse collapse w-100 navCollapse order-1 order-md-0">
      <ul class="navbar-nav ml-auto text-center">
        <li class="nav-item">
          <a class="nav-link" href="#about" :class="navText">Présentation</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#" :class="navText">Offres</a>
        </li>
      </ul>
    </div>
    <a
      class="navbar-brand text-uppercase font-weight-bold d-flex d-md-block align-items-center mx-md-5"
      href="#"
      :class="navText"
      ><img
        v-if="!scrolled"
        src="../assets/logo.svg"
        width="70"
        height="70"
        class="d-md-block align-top mx-md-auto mr-3"
        alt="Logo Magalhaes Florian"
        id="logo" />
      <img
        v-if="scrolled"
        src="../assets/logoOutline.svg"
        width="70"
        height="70"
        class="d-md-block align-top mx-md-auto mr-3"
        alt=""
        id="logo"
    /></a>
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target=".navCollapse"
      aria-controls="navCollapse"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <i class="fas fa-ellipsis-h" :class="navBtn"></i>
    </button>
    <div class="collapse navbar-collapse w-100 navCollapse order-2 order-md-2">
      <ul class="navbar-nav mr-auto text-center">
        <li class="nav-item">
          <a class="nav-link" href="#" :class="navText">Compétences</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#" :class="navText">Contact</a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavBar",
  data: () => {
    return {
      scrolled: false,
      nav: "nav--notScrolled",
      navBtn: "nav-btn--notScrolled",
      navText: "nav-text--notScrolled",
    };
  },
  methods: {
    onScroll() {
      if (window.pageYOffset > 0) {
        this.scrolled = true;
      } else {
        this.scrolled = false;
      }
    },
  },
  mounted() {
    window.addEventListener("scroll", this.onScroll);
  },
  unmounted() {
    window.removeEventListener("scroll", this.onScroll);
  },
  watch: {
    scrolled() {
      if (this.scrolled) {
        this.nav = "nav--scrolled";
        this.navBtn = "nav-btn--scrolled";
        this.navText = "nav-text--scrolled";
      } else {
        this.nav = "nav--notScrolled";
        this.navBtn = "nav-btn--notScrolled";
        this.navText = "nav-text--notScrolled";
      }
    },
  },
};
</script>

<style scoped lang="scss">
nav {
  ul a {
    transition: all 0.3s ease-in-out;
    &:hover {
      transform: scale(1.2);
    }
  }
  &.nav {
    &--scrolled {
      background-color: #455A64;
      transition: all 1.5s ease;
    }
    &--notScrolled {
      background-color: white;
      transition: all 1.5s ease;
    }
  }
  .nav {
    &-btn--scrolled {
      color: white;
    }
    &-btn--notScrolled {
      color: #455A64;
    }
    &-text--scrolled {
      color: white;
    }
    &-text--notScrolled {
      color: #455A64;
    }
  }
}
</style>
