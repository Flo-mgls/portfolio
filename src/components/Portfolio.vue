<template>
  <section id="portfolio">
    <div class="container">
      <h2 class="text-uppercase mb-1">Portfolio</h2>
      <div class="underline mx-auto mb-5"></div>
      <div class="row justify-content-center">
        <div class="col-12 col-md-6 col-lg-4 my-3">
          <PortfolioItem siteName="Deckgen" githubLink="hey">
            <template v-slot:info>
              ipsum rutrum orci, sagittis tempus lacus enim ac dui. Donec non
              enim in turpis pulvinar facilisis.
            </template>
            <template v-slot:techno>
              <i
                class="fab fa-git-alt fa-2x"
                aria-hidden="true"
                title="Git"
              ></i>
              <span class="sr-only">Git</span>
              <i
                class="fab fa-git-alt fa-2x"
                aria-hidden="true"
                title="Git"
              ></i>
              <span class="sr-only">Git</span>
              <i
                class="fab fa-git-alt fa-2x"
                aria-hidden="true"
                title="Git"
              ></i>
              <span class="sr-only">Git</span>
            </template>
          </PortfolioItem>
        </div>
        <div class="col-12 col-md-6 col-lg-4 my-3">
         <PortfolioItem siteName="Deckgen" githubLink="hey">
            <template v-slot:info>
              ipsum rutrum orci, sagittis tempus lacus enim ac dui. Donec non
              enim in turpis pulvinar facilisis.
            </template>
            <template v-slot:techno>
              <i
                class="fab fa-git-alt fa-2x"
                aria-hidden="true"
                title="Git"
              ></i>
              <span class="sr-only">Git</span>
              <i
                class="fab fa-git-alt fa-2x"
                aria-hidden="true"
                title="Git"
              ></i>
              <span class="sr-only">Git</span>
              <i
                class="fab fa-git-alt fa-2x"
                aria-hidden="true"
                title="Git"
              ></i>
              <span class="sr-only">Git</span>
            </template>
          </PortfolioItem>
        </div>
        <div class="col-12 col-md-6 col-lg-4 my-3">
         <PortfolioItem siteName="Deckgen" githubLink="hey">
            <template v-slot:info>
              ipsum rutrum orci, sagittis tempus lacus enim ac dui. Donec non
              enim in turpis pulvinar facilisis.
            </template>
            <template v-slot:techno>
              <i
                class="fab fa-git-alt fa-2x"
                aria-hidden="true"
                title="Git"
              ></i>
              <span class="sr-only">Git</span>
              <i
                class="fab fa-git-alt fa-2x"
                aria-hidden="true"
                title="Git"
              ></i>
              <span class="sr-only">Git</span>
              <i
                class="fab fa-git-alt fa-2x"
                aria-hidden="true"
                title="Git"
              ></i>
              <span class="sr-only">Git</span>
            </template>
          </PortfolioItem>
        </div>
      </div>
    </div>
  </section>
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
