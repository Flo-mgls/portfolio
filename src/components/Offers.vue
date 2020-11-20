<template>
  <!-- OFFERS -->
  <section id="offers">
    <div class="container-fluid">
      <!-- INFO OFFERS -->
      <div class="row">
        <div class="col-md-8 col-lg-6 px-4 px-md-5 py-5 offers-intro">
          <h2 class="text-uppercase mb-4">La solution qui vous convient...</h2>
          <p>
            Pellentesque habitant morbi tristique senectus et netus et malesuada
            fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae,
            ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam
            egestas semper. Aenean ultricies mi vitae est. Mauris placerat
            eleifend leo. Quisque sit amet est et sapien ullamcorper pharetra.
            Vestibulum erat wisi, condimentum sed, commodo vitae.
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
              class="flipCard--back d-flex align-items-center justify-content-center px-2"
            >
              <p>
                Pellentesque habitant morbi tristique senectus et netus et
                malesuada fames ac turpis egestas. Vestibulum tortor quam,
                feugiat vitae.
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
              class="flipCard--back d-flex align-items-center justify-content-center px-2"
            >
              <p>
                Pellentesque habitant morbi tristique senectus et netus et
                malesuada fames ac turpis egestas. Vestibulum tortor quam,
                feugiat vitae.
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
              class="flipCard--back d-flex align-items-center justify-content-center px-2"
            >
              <p>
                Pellentesque habitant morbi tristique senectus et netus et
                malesuada fames ac turpis egestas. Vestibulum tortor quam,
                feugiat vitae.
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
        height: 200px;
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
