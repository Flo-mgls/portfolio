<template>
  <!-- SKILLS -->
  <section id="skills">
    <div class="container-fluid">
      <div class="row align-items-center">
        <!-- SKILLS INFO -->
        <div
          class="col-lg-6 col-md-5 offset-md-1 order-md-last px-4 px-md-5 py-5 skills-intro"
        >
          <h2 class="text-uppercase mb-4">Mes compétences sont vôtres...</h2>
          <p>
            Une bonne présence numérique est une présence qui reflète la qualité
            de vos services, mais pas seulement. Votre
            <strong>site web</strong> sera la première image que votre client
            verra, celui-ci se doit d'être à la hauteur. J'utilise pour cela les
            <b>dernières technologies</b> disponibles pour lesquelles je fais en
            sorte d'être constamment à jour afin de vous fournir un
            <strong>site web</strong> <b>facilement maintenable</b> dans le
            temps mais aussi et surtout qui
            <b>respecte les bonnes normes</b> mises en place par la <b>W3C</b>
            (organisme crée par Tim Berners-Lee, l'homme à l'origine du web).
            <br />
            <br />
            Afin d'être bien référencé, Google prend en compte plusieurs
            critères, il y a bien sûr les <b>mots-clés</b> qui ont une grande
            importance, mais aussi <b>l'adaptabilité du site</b> à différents
            supports, notamment aux mobiles: étant donné qu'aujourd'hui la
            majorité des sites sont consultés sur mobile, Google y accorde
            beaucoup d'importance. Enfin un autre point important est la
            <b>vitesse d'affichage</b> de votre site: Google ne veut pas que ses
            utilisateurs se retrouvent à attendre à cause d'un site peu optimisé
            et ceci jouera donc sur son référencement.
            <br />
            <br />
            <b
              >Vous l'aurez compris, développer votre site, oui, mais surtout:
              le développer en respectant tous ces points et bien d'autres.</b
            >
          </p>
        </div>
        <!-- END SKILLS INFO -->
        <!-- SKILLS CAROUSEL  -->
        <div
          class="col-lg-4 col-md-5 offset-md-1 order-md-first position-relative"
        >
          <div class="skills-list">
            <splide :options="options">
              <!-- CAROUSEL PAGE 1 - LANGAGES -->
              <splide-slide>
                <div class="container skills-list--langages pb-4">
                  <span class="sr-only">Technologies</span>
                  <div class="row my-4">
                    <div class="col-5 text-right">
                      <i
                        class="fab fa-html5 fa-4x"
                        aria-hidden="true"
                        title="HTML"
                      ></i>
                      <span class="sr-only">HTML</span>
                    </div>
                    <div class="col-2"></div>
                    <div class="col-5 text-left">
                      <i
                        class="fab fa-css3-alt fa-4x"
                        aria-hidden="true"
                        title="CSS"
                      ></i>
                      <span class="sr-only">CSS</span>
                    </div>
                  </div>
                  <div class="row my-4">
                    <div class="col-4">
                      <i
                        class="fab fa-js-square fa-4x"
                        aria-hidden="true"
                        title="JavaScript"
                      ></i>
                      <span class="sr-only">JavaScript</span>
                    </div>
                    <div class="col-4">
                      <i
                        class="fab fa-bootstrap fa-4x"
                        aria-hidden="true"
                        title="Bootstrap"
                      ></i>
                      <span class="sr-only">Bootstrap</span>
                    </div>
                    <div class="col-4">
                      <i
                        class="fab fa-wordpress fa-4x"
                        aria-hidden="true"
                        title="Wordpress"
                      ></i>
                      <span class="sr-only">Wordpress</span>
                    </div>
                  </div>
                  <div class="row my-4">
                    <div class="col-4">
                      <i
                        class="fab fa-node fa-4x"
                        aria-hidden="true"
                        title="Node.js"
                      ></i>
                      <span class="sr-only">Node.js</span>
                    </div>
                    <div class="col-4">
                      <i
                        class="fas fa-database fa-4x"
                        aria-hidden="true"
                        title="SQL"
                      ></i>
                      <span class="sr-only">SQL</span>
                    </div>
                    <div class="col-4">
                      <i
                        class="fab fa-sass fa-4x"
                        aria-hidden="true"
                        title="Sass"
                      ></i>
                      <span class="sr-only">Sass</span>
                    </div>
                  </div>
                  <div class="row my-4">
                    <div class="col-5 text-right">
                      <i
                        class="fab fa-vuejs fa-4x"
                        aria-hidden="true"
                        title="Vue.js"
                      ></i>
                      <span class="sr-only">Vue.js</span>
                    </div>
                    <div class="col-2"></div>
                    <div class="col-5 text-left">
                      <i
                        class="fab fa-git-alt fa-4x"
                        aria-hidden="true"
                        title="Git"
                      ></i>
                      <span class="sr-only">Git</span>
                    </div>
                  </div>
                </div>
              </splide-slide>
              <!-- END CAROUSEL PAGE 1 - LANGAGES -->
              <!-- CAROUSEL PAGE 2 - INFOS -->
              <splide-slide>
                <div class="skills-intro--infos pb-4 px-2">
                  <h3 class="text-uppercase my-4">Un gage de qualité...</h3>
                  <ul class="list-group list-group-flush">
                    <li class="list-group-item">Code propre et maintenable</li>
                    <li class="list-group-item">Respect des règles W3C</li>
                    <li class="list-group-item">
                      Design adapté sur tous les appareils
                    </li>
                    <li class="list-group-item">
                      Respect des règles WCAG (accessibilité)
                    </li>
                    <li class="list-group-item">
                      Méthodes propres pour un bon référencement (SEO)
                    </li>
                    <li class="list-group-item">
                      Sécurisé (OWASP) et respect du RGPD
                    </li>
                  </ul>
                </div>
              </splide-slide>
              <!-- END CAROUSEL PAGE 2 - INFOS -->
            </splide>
          </div>
        </div>
        <!-- END SKILLS CAROUSEL  -->
      </div>
    </div>
  </section>
  <!-- END SKILLS -->
</template>

<script>
import { Splide, SplideSlide } from "@splidejs/vue-splide";
import "@splidejs/splide/dist/css/themes/splide-default.min.css";

export default {
  name: "Skills",
  components: {
    Splide,
    SplideSlide,
  },
  data() {
    return {
      options: {
        rewind: true,
        width: 800,
        gap: "1rem",
        arrows: false,
        pagination: true,
        perPage: 1,
      },
    };
  },
};
</script>

<style scoped lang="scss">
#skills {
  padding-top: 6em;
  .position-relative {
    top: -80px;
  }
  @media screen and (min-width: 768px) {
    .position-relative {
      top: 0px;
    }
  }
  .skills {
    &-intro {
      background-color: #455a64;
      color: white;
      border: 1px solid #455a64;
      padding-bottom: 6em !important;
      @media screen and (min-width: 768px) {
        border-radius: 10px 0 0 10px;
      }
    }
    &-list {
      border-radius: 10px;
      box-shadow: 0px 25px 40px rgba(0, 0, 0, 0.2);
      background-color: white;
    }
  }
}
li {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
