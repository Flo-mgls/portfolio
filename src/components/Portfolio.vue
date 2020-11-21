<template>
  <!-- PORTFOLIO -->
  <section id="portfolio">
    <div class="container">
      <h2 class="text-uppercase mb-1">Réalisations</h2>
      <div class="underline mx-auto mb-5"></div>
      <div class="row justify-content-center">
        <!-- ITEM 1 -->
        <div class="col-12 col-md-6 col-lg-4 my-3">
          <PortfolioItem
            siteName="Ce site"
            githubLink="https://github.com/Flo-mgls/Portfolio"
            siteLink="https://florian-magalhaes.fr"
          >
            <template v-slot:info> Ce site, réalisé avec Vue.js </template>
            <template v-slot:techno>
              <i class="fab fa-html5 fa-2x" aria-hidden="true" title="HTML"></i>
              <span class="sr-only">HTML</span>
              <i
                class="fab fa-css3-alt fa-2x"
                aria-hidden="true"
                title="CSS"
              ></i>
              <span class="sr-only">CSS</span>
              <i
                class="fab fa-js-square fa-2x"
                aria-hidden="true"
                title="JavaScript"
              ></i>
              <span class="sr-only">JavaScript</span>
              <i
                class="fab fa-bootstrap fa-2x"
                aria-hidden="true"
                title="Bootstrap"
              ></i>
              <span class="sr-only">Bootstrap</span>
              <i
                class="fab fa-vuejs fa-2x"
                aria-hidden="true"
                title="Vue.js"
              ></i>
              <span class="sr-only">Vue.js</span>
              <i class="fab fa-sass fa-2x" aria-hidden="true" title="Sass"></i>
              <span class="sr-only">Sass</span>
            </template>
          </PortfolioItem>
        </div>
        <!-- END ITEM 1 -->
        <!-- ITEM 2 -->
        <div class="col-12 col-md-6 col-lg-4 my-3">
          <PortfolioItem
            siteName="Deckgen"
            githubLink="https://github.com/Flo-mgls/deckGen"
            siteLink="https://florian-magalhaes.fr/deckGen/"
          >
            <template v-slot:info>
              Générateur de deck pour un jeu en ligne: Clash Royale
            </template>
            <template v-slot:techno>
              <i class="fab fa-html5 fa-2x" aria-hidden="true" title="HTML"></i>
              <span class="sr-only">HTML</span>
              <i
                class="fab fa-css3-alt fa-2x"
                aria-hidden="true"
                title="CSS"
              ></i>
              <span class="sr-only">CSS</span>
              <i
                class="fab fa-js-square fa-2x"
                aria-hidden="true"
                title="JavaScript"
              ></i>
              <span class="sr-only">JavaScript</span>
              <i
                class="fab fa-bootstrap fa-2x"
                aria-hidden="true"
                title="Bootstrap"
              ></i>
              <span class="sr-only">Bootstrap</span>
              <i
                class="fab fa-vuejs fa-2x"
                aria-hidden="true"
                title="Vue.js"
              ></i>
            </template>
          </PortfolioItem>
        </div>
        <!-- END ITEM 2 -->
        <!-- ITEM 3 -->
        <div class="col-12 col-md-6 col-lg-4 my-3">
          <PortfolioItem
            siteName="Groupomania"
            githubLink="https://github.com/Flo-mgls/groupomania"
          >
            <template v-slot:info>
              Réseau social d'entreprise: Création de comptes, pages de profil,
              publications (commentaires et réactions)
            </template>
            <template v-slot:techno>
              <i class="fab fa-html5 fa-1x" aria-hidden="true" title="HTML"></i>
              <span class="sr-only">HTML</span>
              <i
                class="fab fa-css3-alt fa-1x"
                aria-hidden="true"
                title="CSS"
              ></i>
              <span class="sr-only">CSS</span>
              <i
                class="fab fa-js-square fa-1x"
                aria-hidden="true"
                title="JavaScript"
              ></i>
              <span class="sr-only">JavaScript</span>
              <i
                class="fab fa-bootstrap fa-1x"
                aria-hidden="true"
                title="Bootstrap"
              ></i>
              <span class="sr-only">Bootstrap</span>
              <i
                class="fab fa-vuejs fa-1x"
                aria-hidden="true"
                title="Vue.js"
              ></i>
              <span class="sr-only">Vue.js</span>
              <i class="fab fa-sass fa-1x" aria-hidden="true" title="Sass"></i>
              <i
                class="fab fa-node fa-1x"
                aria-hidden="true"
                title="Node.js"
              ></i>
              <span class="sr-only">Node.js</span>
              <i
                class="fas fa-database fa-1x"
                aria-hidden="true"
                title="SQL"
              ></i>
              <span class="sr-only">SQL</span>
            </template>
          </PortfolioItem>
        </div>
        <!-- END ITEM 3 -->
        <!-- ITEM 4 -->
        <div class="col-12 col-md-6 col-lg-4 my-3">
          <PortfolioItem
            siteName="Piquante"
            githubLink="https://github.com/Flo-mgls/piquante-back"
          >
            <template v-slot:info>
              Site de notation de sauces: création de compte, publication de sauces, reactions à celles-ci <br>Backend
            </template>
            <template v-slot:techno>
              <i
                class="fab fa-js-square fa-2x"
                aria-hidden="true"
                title="JavaScript"
              ></i>
              <span class="sr-only">JavaScript</span>
              <i
                class="fab fa-node fa-2x"
                aria-hidden="true"
                title="Node.js"
              ></i>
              <span class="sr-only">Node.js</span>
            </template>
          </PortfolioItem>
        </div>
        <!-- END ITEM 4 -->
        <!-- ITEM 5 -->
        <div class="col-12 col-md-6 col-lg-4 my-3">
          <PortfolioItem
            siteName="Orinoco"
            githubLink="https://github.com/Flo-mgls/orinoco"
          >
            <template v-slot:info>
              Site de vente d'oursons en peluche: du choix du produit à la confirmation de commande <br>Frontend
            </template>
            <template v-slot:techno>
              <i class="fab fa-html5 fa-2x" aria-hidden="true" title="HTML"></i>
              <span class="sr-only">HTML</span>
              <i
                class="fab fa-css3-alt fa-2x"
                aria-hidden="true"
                title="CSS"
              ></i>
              <span class="sr-only">CSS</span>
              <i
                class="fab fa-js-square fa-2x"
                aria-hidden="true"
                title="JavaScript"
              ></i>
              <span class="sr-only">JavaScript</span>
              <i
                class="fab fa-bootstrap fa-2x"
                aria-hidden="true"
                title="Bootstrap"
              ></i>
              <span class="sr-only">Bootstrap</span>
              <i class="fab fa-sass fa-2x" aria-hidden="true" title="Sass"></i>
              <span class="sr-only">Sass</span>
            </template>
          </PortfolioItem>
        </div>
        <!-- END ITEM 5 -->
        <!-- ITEM 6 -->
        <div class="col-12 col-md-6 col-lg-4 my-3">
          <PortfolioItem siteName="La chouette agence">
            <template v-slot:info>
              Optimisation du site déjà existant: performance d'affichage accrue, design repensé pour s'afficher correctement sur mobile, référencement amélioré
            </template>
            <template v-slot:techno>
              <i class="fab fa-html5 fa-2x" aria-hidden="true" title="HTML"></i>
              <span class="sr-only">HTML</span>
              <i
                class="fab fa-css3-alt fa-2x"
                aria-hidden="true"
                title="CSS"
              ></i>
              <span class="sr-only">CSS</span>
            </template>
          </PortfolioItem>
        </div>
        <!-- END ITEM 6 -->
        <!-- ITEM 7 -->
        <div class="col-12 col-md-6 col-lg-4 my-3">
          <PortfolioItem
            siteName="Ohmyfood"
            githubLink="https://github.com/Flo-mgls/ohmyfood"
          >
            <template v-slot:info>
              Site de présentation de menu d'un restaurant: intégration d'une maquette, animation ajoutée
            </template>
            <template v-slot:techno>
              <i class="fab fa-html5 fa-2x" aria-hidden="true" title="HTML"></i>
              <span class="sr-only">HTML</span>
              <i
                class="fab fa-css3-alt fa-2x"
                aria-hidden="true"
                title="CSS"
              ></i>
              <span class="sr-only">CSS</span>
              <i class="fab fa-sass fa-2x" aria-hidden="true" title="Sass"></i>
              <span class="sr-only">Sass</span>
            </template>
          </PortfolioItem>
        </div>
        <!-- END ITEM 7 -->
      </div>
    </div>
  </section>
  <!-- END PORTFOLIO -->
</template>

<script>
import PortfolioItem from "./PortfolioItem.vue";

export default {
  name: "Portfolio",
  components: {
    PortfolioItem,
  },
};
</script>

<style scoped lang="scss">
#portfolio {
  padding-top: 6em;
  .underline {
    height: 2px;
    width: 50px;
    border-radius: 15px;
    background-color: #9eadb5;
  }
}
</style>
