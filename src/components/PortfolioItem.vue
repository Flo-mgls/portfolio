<template>
  <!-- PORTFOLIO ITEM -->
  <div class="portfolio-item">
    <div class="flipCard">
      <!-- FRONT - SITE NAME -->
      <div
        class="flipCard--front d-flex align-items-center justify-content-center px-1"
      >
        <h3 class="text-uppercase">{{ siteName }}</h3>
        <i
          class="fas fa-fingerprint fa-lg position-absolute"
          aria-hidden="true"
        ></i>
      </div>
      <!-- END FRONT - SITE NAME -->
      <!-- BACK - SITE INFO -->
      <div
        class="flipCard--back d-flex align-items-center justify-content-center p-2"
      >
        <div class="row align-items-center justify-content-center mb-2">
          <div class="col-9">
            <div class="row">
              <div class="col-12">
                <p>
                  <slot name="info"></slot>
                </p>
              </div>
              <div
                class="col-12 d-flex align-items-center justify-content-around"
              >
                <slot name="techno"></slot>
              </div>
            </div>
          </div>
          <div
            class="col-3 d-flex align-items-center justify-content-center flex-column"
            v-if="githubLink || siteLink"
          >
            <a :href="githubLink" class="py-2" v-if="githubLink"
              ><i
                class="fab fa-github-alt fa-3x"
                aria-hidden="true"
                title="Lien Github"
              ></i
              ><span class="sr-only">Lien Github</span></a
            >
            <a :href="siteLink" class="py-2" v-if="siteLink"
              ><i
                class="fas fa-search fa-3x"
                aria-hidden="true"
                title="Lien du site"
              ></i
              ><span class="sr-only">Lien du site</span></a
            >
          </div>
        </div>
      </div>
      <!-- END BACK - SITE INFO -->
    </div>
  </div>
  <!-- END PORTFOLIO ITEM -->
</template>

<script>
export default {
  name: "PortfolioItem",
  props: {
    siteName: {
      type: String,
      required: true,
    },
    githubLink: {
      type: String,
    },
    siteLink: {
      type: String,
    },
  },
};
</script>

<style scoped lang="scss">
.portfolio-item {
  background-color: transparent;
  width: auto;
  height: 250px;
  perspective: 1000px;
  &:hover .flipCard {
    transform: rotateY(180deg);
  }
  .flipCard {
    position: relative;
    width: 100%;
    height: 100%;
    transition: transform 0.8s;
    transform-style: preserve-3d;
    .fa-fingerprint {
      color: #9eadb5;
      bottom: 10px;
      right: 10px;
    }
    a {
      color: #9eadb5;
      &:hover {
        color: #455a64;
      }
    }
    &--front,
    &--back {
      position: absolute;
      width: 100%;
      height: 100%;
      -webkit-backface-visibility: hidden;
      backface-visibility: hidden;
      border-radius: 10px;
      box-shadow: 0px 25px 40px rgba(0, 0, 0, 0.2);
      background-color: white;
    }
    &--back {
      transform: rotateY(180deg);
    }
  }
}
</style>
