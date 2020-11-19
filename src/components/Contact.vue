<template>
  <section id="contact">
    <div class="container-fluid contact p-3">
      <div class="row">
        <div class="col-6 col-md-3">
          <a href="mailto:m.f.pro@outlook.com"
            ><i
              class="fas fa-envelope fa-3x d-block mb-1 mt-4 mt-md-1"
              aria-hidden="true"
              title="Email"
            ></i
            ><span class="sr-only">Email</span>m.f.pro@outlook.com</a
          >
        </div>
        <div class="col-6 col-md-3 order-md-last">
          <a href="tel:0668886240"
            ><i
              class="fas fa-mobile-alt fa-3x d-block mb-1 mt-4 mt-md-1"
              aria-hidden="true"
              title="Mobile"
            ></i
            ><span class="sr-only">Mobile</span>06 68 88 62 40</a
          >
        </div>
        <div class="col-6 col-md-3">
          <a href="https://www.linkedin.com/in/florian-magalhaes/"
            ><i
              class="fab fa-linkedin-in fa-3x d-block mb-1 mt-4 mt-md-1"
              aria-hidden="true"
              title="LinkedIn"
            ></i
            ><span class="sr-only">LinkedIn</span>@florian-magalhaes</a
          >
        </div>
        <div class="col-6 col-md-3">
          <a href="https://github.com/Flo-mgls"
            ><i
              class="fab fa-github-alt fa-3x d-block mb-1 mt-4 mt-md-1"
              aria-hidden="true"
              title="Github"
            ></i
            ><span class="sr-only">Github</span>@Flo-mgls</a
          >
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Contact",
};
</script>

<style scoped lang="scss">
#contact {
  padding-top: 6em;
  .contact {
    background-color: #455a64;
    i {
      color: #9eadb5;
      &:hover {
        color: white;
      }
    }
    a {
      @media screen and (max-width: 374px) {
        font-size: 0.7em;
      }
      color: white;
      &:hover {
        text-decoration: none;
      }
    }
  }
}
</style>
