<template>
  <!-- NAV -->
  <nav class="navbar navbar-expand-md fixed-top py-0" :class="nav">
    <!-- LEFT NAV -->
    <div class="navbar-collapse collapse w-100 navCollapse order-1 order-md-0">
      <ul class="navbar-nav ml-auto text-center">
        <li class="nav-item">
          <a class="nav-link" href="#intro" :class="navText">Présentation</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#offers" :class="navText">Offres</a>
        </li>
      </ul>
    </div>
    <!-- END LEFT NAV -->
    <!-- CENTER NAV - LOGO -->
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
    <!-- END CENTER NAV - LOGO -->
    <!-- BUTTON NAV -->
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
    <!-- END BUTTON NAV -->
    <!-- RIGHT NAV -->
    <div class="collapse navbar-collapse w-100 navCollapse order-2 order-md-2">
      <ul class="navbar-nav mr-auto text-center">
        <li class="nav-item">
          <a class="nav-link" href="#skills" :class="navText">Compétences</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#portfolio" :class="navText">Portfolio</a>
        </li>
      </ul>
    </div>
    <!-- END RIGHT NAV -->
    <!-- CONTACT NAV -->
    <div class="collapse navbar-collapse navCollapse order-3 nav-contact">
      <ul class="navbar-nav mr-auto text-center">
        <li class="nav-item">
          <a class="nav-link nav-contact--link" href="#contact" :class="navText"
            >Contact</a
          >
        </li>
      </ul>
    </div>
    <!-- END CONTACT NAV -->
  </nav>
  <!-- END NAV -->
</template>

<script>
export default {
  name: "NavBar",
  data: () => {
    return {
      scrolled: false, //If page has been scrolled
      nav: "nav--notScrolled",
      navBtn: "nav-btn--notScrolled",
      navText: "nav-text--notScrolled",
    };
  },
  methods: {
    onScroll() {
      //Determine if page has been scrolled
      if (window.pageYOffset > 0) {
        this.scrolled = true;
      } else {
        this.scrolled = false;
      }
    },
  },
  mounted() {
    //Trigger method if scroll
    window.addEventListener("scroll", this.onScroll);
  },
  unmounted() {
    window.removeEventListener("scroll", this.onScroll);
  },
  watch: {
    scrolled() {
      //Check if data scrolled have been changed
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
      transform: scale(1.1);
    }
  }
  &.nav {
    &--scrolled {
      background-color: #455a64;
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
      color: #455a64;
    }
    &-text--scrolled {
      color: white;
      border-color: white !important;
    }
    &-text--notScrolled {
      color: #455a64;
    }
    &-contact {
      @media screen and (min-width: 768px) {
        position: absolute;
        right: 20px;
        .nav-contact--link {
          border-radius: 30px;
          border: 1px solid #455a64;
          &:hover {
            background-color: #455a64;
            color: white;
          }
        }
      }
    }
  }
}
</style>
