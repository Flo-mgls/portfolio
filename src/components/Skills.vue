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
            Pellentesque habitant morbi tristique senectus et netus et malesuada
            fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae,
            ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam
            egestas semper. Aenean ultricies mi vitae est. Mauris placerat
            eleifend leo. Quisque sit amet est et sapien ullamcorper pharetra.
            Vestibulum erat wisi, condimentum sed, commodo vitae.
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
                    <div class="col-4">
                      <i
                        class="fab fa-html5 fa-4x"
                        aria-hidden="true"
                        title="HTML"
                      ></i>
                      <span class="sr-only">HTML</span>
                    </div>
                    <div class="col-4">
                      <i
                        class="fab fa-css3-alt fa-4x"
                        aria-hidden="true"
                        title="CSS"
                      ></i>
                      <span class="sr-only">CSS</span>
                    </div>
                    <div class="col-4">
                      <i
                        class="fab fa-js-square fa-4x"
                        aria-hidden="true"
                        title="JavaScript"
                      ></i>
                      <span class="sr-only">JavaScript</span>
                    </div>
                  </div>
                  <div class="row my-4">
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
                        class="fab fa-vuejs fa-4x"
                        aria-hidden="true"
                        title="Vue.js"
                      ></i>
                      <span class="sr-only">Vue.js</span>
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
