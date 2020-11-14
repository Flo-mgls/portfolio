<template>
  <nav class="navbar navbar-expand-md navbar-light bg-light">
    <div
      class="navbar-collapse collapse w-100 navCollapse order-1 order-md-0"
    >
      <ul class="navbar-nav ml-auto text-center">
        <li class="nav-item">
          <a class="nav-link" href="#">Présentation</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Offres</a>
        </li>
      </ul>
    </div>
    <a
      class="navbar-brand text-uppercase d-flex d-md-block align-items-center mx-md-5"
      href="#"
      ><img
        src="../assets/logo.svg"
        width="50"
        height="50"
        class="d-md-block align-top mx-md-auto mr-3"
        alt=""
        id="logo"
      />Magalhaes Florian</a
    >
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target=".navCollapse"
      aria-controls="navCollapse"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <div
      class="collapse navbar-collapse w-100 navCollapse order-2 order-md-2"
    >
      <ul class="navbar-nav mr-auto text-center">
        <li class="nav-item">
          <a class="nav-link" href="#">Compétences</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Contact</a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavBar",
  props: {},
};
</script>

<style scoped>
@media screen and (max-width: 425px) {
  img {
    height: 30px;
    width: 30px;
  }
  button span {
    height: 1em;
    width: 1em;
  }
  a {
    font-size: 1em;
  }
}
</style>
