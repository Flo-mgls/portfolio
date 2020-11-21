<template>
  <!-- OFFERS -->
  <section id="offers">
    <div class="container-fluid">
      <!-- INFO OFFERS -->
      <div class="row">
        <div class="col-md-8 col-lg-6 px-4 px-md-5 py-5 offers-intro">
          <h2 class="text-uppercase mb-4">La solution qui vous convient...</h2>
          <p>
            Avoir une présence sur le net en 2020 n'est plus une chose à
            négliger et pour certains cela est même une nécessité, surtout en
            ces temps. À différentes idées, différentes solutions, cependant
            pour chacune d'entre elles, la qualité de ma prestation sera mon
            objectif principal. Cela passe bien sûr par le développement de
            votre site, mais aussi et au besoin par la maintenance de celui-ci,
            son évolution au fil de la vôtre et le suivi de ses statistiques.
            <br />
            Mettre en œuvre vos idées, oui, mais le plus important: les perdurer.
          </p>
        </div>
      </div>
      <!-- END INFO OFFERS -->
      <div
        class="row no-gutters justify-content-around position-relative offers-site"
      >
        <!-- FIRST OFFER -->
        <div class="col-md-3 w-100 mb-4 offers-site--1">
          <div class="flipCard">
            <!-- FRONT - OFFER NAME -->
            <div
              class="flipCard--front d-flex align-items-center justify-content-center px-1"
            >
              <h3 class="text-uppercase">Site vitrine</h3>
              <i
                class="fas fa-fingerprint fa-lg position-absolute"
                aria-hidden="true"
              ></i>
            </div>
            <!-- FRONT - OFFER NAME -->
            <!-- BACK - OFFER INFO -->
            <div
              class="flipCard--back d-flex align-items-center justify-content-center p-2"
            >
              <p>
                Vous avez une entreprise et souhaitez être <strong>présent sur le web</strong> ?
                <br />
                La possibilité d'être trouvé par vos futurs clients, la
                présentation de vos différents services ou alors tout simplement
                une idée que vous avez envie de partager...
                <br />
                Un <strong>site vitrine</strong> est la solution la plus commune mais aussi la
                plus efficace
              </p>
            </div>
            <!-- BACK - OFFER INFO -->
          </div>
        </div>
        <!-- END FIRST OFFER -->
        <!-- SECOND OFFER -->
        <div class="col-md-3 w-100 mb-4 offers-site--2">
          <div class="flipCard">
            <!-- FRONT - OFFER NAME -->
            <div
              class="flipCard--front d-flex align-items-center justify-content-center px-1"
            >
              <h3 class="text-uppercase">Site e-commerce</h3>
              <i
                class="fas fa-fingerprint fa-lg position-absolute"
                aria-hidden="true"
              ></i>
            </div>
            <!-- END FRONT - OFFER NAME -->
            <!-- BACK - OFFER INFO -->
            <div
              class="flipCard--back d-flex align-items-center justify-content-center p-2"
            >
              <p>
                Le cœur de votre entreprise est de vendre différents produits et
                vous souhaitez avoir une présence dans le plus grand marché de
                notre siècle, le web ? Un <strong>site e-commerce</strong>, lorsque votre but est
                de proposer et vendre vos produits, est indispensable.
                <br />
                En 2019, <b>87,5%</b> des internautes français ont acheté en ligne
              </p>
            </div>
            <!-- END BACK - OFFER INFO -->
          </div>
        </div>
        <!-- END SECOND OFFER -->
        <!-- THIRD OFFER -->
        <div class="col-md-3 w-100 offers-site--3">
          <div class="flipCard">
            <!-- FRONT - OFFER NAME -->
            <div
              class="flipCard--front d-flex align-items-center justify-content-center px-1"
            >
              <h3 class="text-uppercase">Site dynamique</h3>
              <i
                class="fas fa-fingerprint fa-lg position-absolute"
                aria-hidden="true"
              ></i>
            </div>
            <!-- END FRONT - OFFER NAME -->
            <!-- BACK - OFFER INFO -->
            <div
              class="flipCard--back d-flex align-items-center justify-content-center p-2"
            >
              <p>
                Votre projet ne rentre ni dans le cadre d'un <strong>site vitrine</strong> ni
                dans celui d'un <strong>site e-commerce</strong> ?
                <br />
                Un réseau social, un outil, ou autre chose... Tout peut être
                imaginé, tout peut être développé, n'hésitez pas à prendre
                contact afin de discuter de votre <b>projet</b>
              </p>
            </div>
            <!-- END BACK - OFFER INFO -->
          </div>
        </div>
        <!-- END THIRD OFFER -->
      </div>
    </div>
  </section>
  <!-- END OFFERS -->
</template>

<script>
export default {
  name: "Offers",
};
</script>

<style scoped lang="scss">
#offers {
  padding-top: 6em;
  .offers {
    &-intro {
      background-color: #455a64;
      color: white;
      border: 1px solid #455a64;
      padding-bottom: 6em !important;
      @media screen and (min-width: 768px) {
        border-radius: 0 10px 10px 0;
      }
    }
    &-site {
      top: -80px;
      &--1,
      &--2,
      &--3 {
        background-color: transparent;
        width: auto;
        height: 260px;
        @media screen and (min-width: 768px) {
          height: 450px;
        }
        perspective: 1000px;
        &:hover .flipCard {
          transform: rotateY(180deg);
        }
      }
      .flipCard {
        position: relative;
        width: 100%;
        height: 100%;
        transition: transform 0.8s;
        transform-style: preserve-3d;
        i {
          color: #9eadb5;
          bottom: 10px;
          right: 10px;
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
  }
}
</style>
