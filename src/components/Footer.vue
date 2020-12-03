<template>
  <!-- FOOTER INFO -->
  <section id="footer" class="pt-3">
    <div class="container-fluid">
      <p class="mb-0">
        Copyright © 2020 Tous droits réservés | Florian Magalhaes
      </p>
      <button
        type="button"
        data-toggle="collapse"
        data-target="#collapseMentions"
        aria-expanded="false"
        aria-controls="collapseMentions"
      >
        Mentions Légales
      </button>
      <div class="collapse" id="collapseMentions">
        <p class="mb-0 mt-2">
          <b>Propriétaire</b> : Florian Magalhaes – 888631660 – 1625
          rue du Chêne couronné, 71600 Vitry en charollais<br />
          <b>Créateur</b> : Florian Magalhaes<br />
          <b>Responsable publication</b> : Florian Magalhaes –
          m.f.pro@outlook.com<br />
          Le responsable publication est une personne physique ou une personne
          morale.<br />
          <b>Webmaster</b> : Florian Magalhaes –
          m.f.pro@outlook.com<br />
          <b>Hébergeur</b> : GANDI SAS – 63-65 boulevard Massena Paris
          (75013) FRANCE
        </p>
      </div>
    </div>
  </section>
  <!-- END FOOTER INFO -->
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped lang="scss">
#footer {
  background-color: #455a64;
  color: white;
  font-size: 0.8em;
  @media screen and (max-width: 374px) {
    font-size: 0.6em;
  }
  button {
    background: none;
    color: inherit;
    border: none;
    padding: 0;
    font: inherit;
    cursor: pointer;
    outline: inherit;
  }
}
</style>
