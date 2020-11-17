<template>
  <section id="about">
    <div class="container">
      <div class="row no-gutters">
        <div class="col-lg-6 col-md-4 position-relative">
          <div class="intro-logo position-absolute">
            <img
              src="../assets/logoMF.svg"
              alt="Lettres M et F superposées sur le logo de Magalhaes Florian "
            />
          </div>
        </div>
        <div class="intro-text col-lg-6 col-md-8 px-4 px-md-5 py-5">
          <h2 class="intro-text--title text-uppercase mb-4">
            Votre développeur...
          </h2>
          <p>
            Pellentesque habitant morbi tristique senectus et netus et malesuada
            fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae,
            ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam
            egestas semper. Aenean ultricies mi vitae est. Mauris placerat
            eleifend leo. Quisque sit amet est et sapien ullamcorper pharetra.
            Vestibulum erat wisi, condimentum sed, commodo vitae, ornare sit
            amet, wisi. Aenean fermentum, elit eget tincidunt condimentum, eros
            ipsum rutrum orci, sagittis tempus lacus enim ac dui. Donec non enim
            in turpis pulvinar facilisis. Ut felis. Praesent dapibus, neque id
            cursus faucibus, tortor neque egestas augue.
          </p>
          <a
            class="btn text-uppercase"
            href="/CVMagalhaesFlorian.pdf"
            role="button"
            >CV Complet</a
          >
        </div>
      </div>
      <br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
      <p>
        Pellentesque habitant morbi tristique senectus et netus et malesuada
        fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae,
        ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam
        egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend
        leo. Quisque sit amet est et sapien ullamcorper pharetra. Vestibulum
        erat wisi, condimentum sed, commodo vitae, ornare sit amet, wisi. Aenean
        fermentum, elit eget tincidunt condimentum, eros ipsum rutrum orci,
        sagittis tempus lacus enim ac dui. Donec non enim in turpis pulvinar
        facilisis. Ut felis. Praesent dapibus, neque id cursus faucibus, tortor
        neque egestas augue, eu vulputate magna eros eu erat. Aliquam erat
        volutpat. Nam dui mi, tincidunt quis, accumsan porttitor, facilisis
        luctus, metus
      </p>
      <p>
        Pellentesque habitant morbi tristique senectus et netus et malesuada
        fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae,
        ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam
        egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend
        leo. Quisque sit amet est et sapien ullamcorper pharetra. Vestibulum
        erat wisi, condimentum sed, commodo vitae, ornare sit amet, wisi. Aenean
        fermentum, elit eget tincidunt condimentum, eros ipsum rutrum orci,
        sagittis tempus lacus enim ac dui. Donec non enim in turpis pulvinar
        facilisis. Ut felis. Praesent dapibus, neque id cursus faucibus, tortor
        neque egestas augue, eu vulputate magna eros eu erat. Aliquam erat
        volutpat. Nam dui mi, tincidunt quis, accumsan porttitor, facilisis
        luctus, metus
      </p>
      <p>
        Pellentesque habitant morbi tristique senectus et netus et malesuada
        fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae,
        ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam
        egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend
        leo. Quisque sit amet est et sapien ullamcorper pharetra. Vestibulum
        erat wisi, condimentum sed, commodo vitae, ornare sit amet, wisi. Aenean
        fermentum, elit eget tincidunt condimentum, eros ipsum rutrum orci,
        sagittis tempus lacus enim ac dui. Donec non enim in turpis pulvinar
        facilisis. Ut felis. Praesent dapibus, neque id cursus faucibus, tortor
        neque egestas augue, eu vulputate magna eros eu erat. Aliquam erat
        volutpat. Nam dui mi, tincidunt quis, accumsan porttitor, facilisis
        luctus, metus
      </p>
      <p>
        Pellentesque habitant morbi tristique senectus et netus et malesuada
        fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae,
        ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam
        egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend
        leo. Quisque sit amet est et sapien ullamcorper pharetra. Vestibulum
        erat wisi, condimentum sed, commodo vitae, ornare sit amet, wisi. Aenean
        fermentum, elit eget tincidunt condimentum, eros ipsum rutrum orci,
        sagittis tempus lacus enim ac dui. Donec non enim in turpis pulvinar
        facilisis. Ut felis. Praesent dapibus, neque id cursus faucibus, tortor
        neque egestas augue, eu vulputate magna eros eu erat. Aliquam erat
        volutpat. Nam dui mi, tincidunt quis, accumsan porttitor, facilisis
        luctus, metus
      </p>
    </div>
  </section>
</template>

<script>
export default {
  name: "Intro",
};
</script>

<style scoped lang="scss">
@media screen and (min-width: 768px) and (max-width: 991px) {
  img {
    height: 290px;
    width: 290px;
  }
  .intro-logo {
    top: 100px;
    left: -10px;
    z-index: 1;
  }
}
@media screen and (min-width: 992px) and (max-width: 1199px) {
  img {
    height: 410px;
    width: 410px;
  }
  .intro-logo {
    top: 50px;
    left: 100px;
    z-index: 1;
  }
}
@media screen and (min-width: 1200px) {
  img {
    height: 500px;
    width: 500px;
  }
  .intro-logo {
    top: 0px;
    left: 100px;
    z-index: 1;
  }
}
@media screen and (max-width: 375px) {
  h2 {
    font-size: 1.5em;
  }
}
section {
  padding-top: 6em;
}
.intro-text {
  border-radius: 10px;
  border: 1px solid #455A64;
  box-shadow: 0px 25px 40px rgba(0, 0, 0, 0.2);
}
a {
  color: #455A64;
  border-radius: 30px;
  border: 1px solid #455A64;
  &:hover {
    background-color: #455A64;
    color: white;
  }
}
</style>
