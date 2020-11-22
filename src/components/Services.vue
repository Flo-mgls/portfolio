<template>
  <!-- HEADER -->
  <section id="services">
    <div class="container-fluid">
      <div class="row">
        <div class="col-6 col-md-4 col-lg-2 p-3 border-right">
          <i
            class="far fa-check-circle fa-3x d-block mb-3"
            aria-hidden="true"
          ></i>
          Design adapté à tous types d'appareils
        </div>
        <div class="col-6 col-md-4 col-lg-2 p-3 border-right">
          <i
            class="far fa-check-circle fa-3x d-block mb-3"
            aria-hidden="true"
          ></i>
          Optimisation pour une vitesse d'affichage optimale
        </div>
        <div class="col-6 col-md-4 col-lg-2 p-3 border-right">
          <i
            class="far fa-check-circle fa-3x d-block mb-3"
            aria-hidden="true"
          ></i
          >Sécurisé
        </div>
        <div class="col-6 col-md-4 col-lg-2 p-3 border-right">
          <i
            class="far fa-check-circle fa-3x d-block mb-3"
            aria-hidden="true"
          ></i
          >Hébergement
        </div>
        <div class="col-6 col-md-4 col-lg-2 p-3 border-right">
          <i
            class="far fa-check-circle fa-3x d-block mb-3"
            aria-hidden="true"
          ></i>
          Référencement sur vos mots-clés
        </div>
        <div class="col-6 col-md-4 col-lg-2 p-3">
          <i
            class="far fa-check-circle fa-3x d-block mb-3"
            aria-hidden="true"
          ></i>
          Maintenance d'un an offerte
        </div>
      </div>
    </div>
  </section>
  <!-- END HEADER -->
</template>

<script>
export default {
  name: "Services",
};
</script>

<style scoped lang="scss">
#services {
  @media screen and (min-width: 768px) {
    padding-top: 8em;
  }
  padding-top: 3em;
}
</style>
