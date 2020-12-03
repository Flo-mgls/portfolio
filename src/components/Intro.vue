<template>
  <!-- INTRO -->
  <section id="intro">
    <div class="container">
      <div class="row no-gutters">
        <!-- LOGO  -->
        <div class="col-lg-6 col-md-4 position-relative">
          <div class="intro-logo position-absolute">
            <img
              src="../assets/logoMF.svg"
              alt="Lettres M et F superposées sur le logo de Magalhaes Florian "
            />
          </div>
        </div>
        <!-- END LOGO -->
        <!-- PRESENTATION -->
        <div class="intro-text col-lg-6 col-md-8 px-4 px-md-5 py-5">
          <h2 class="text-uppercase mb-4">Votre développeur...</h2>
          <p>
            Mes premiers pas dans l'informatique remontent à 5 ans où j'avais
            mis en ligne sur le Google Play deux petits jeux mobiles, la
            création et ce qu'on ressent lorsque celle-ci est en ligne et
            fonctionne absolument comme nous l'avons prévu, est sans aucun doute
            l'une des choses qui m'a le plus plu.
            <br />
            En arrivant dans le supérieur j'ai choisi d'étudier la biologie,
            une autre de mes grandes passions: la science. Toutefois <strong>l'informatique</strong>
            ne m'a jamais quitté et j'ai commencé à suivre des cours dans le
            domaine du <strong>développement web</strong>, voyant que cela me plaisait énormément
            j'ai alors entrepris de valider mes acquis à l'aide d'un diplôme que
            j'ai obtenu en octobre 2020: <strong>Développeur web full stack</strong>.
            <br /><br />
            <b>Je vous propose donc mon savoir-faire, celui-ci en phase avec les
            dernières lignes directives du développement, afin de vous aider à
            vous faire une présence dans cet énorme monde qu'est le web.</b>
            <br /><br />
            Je suis disponible pour travailler avec vous à distance, partout
            dans le monde, avec la possibilité de se rencontrer si vous êtes en
            <strong>Bourgogne et dans les villes alentours telles que Dijon et Lyon.</strong>
          </p>
          <a
            class="btn text-uppercase"
            href="https://www.linkedin.com/in/florian-magalhaes/"
            role="button"
            >LinkedIn</a
          >
        </div>
        <!-- END PRESENTATION -->
      </div>
    </div>
  </section>
  <!-- END INTRO -->
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
    top: 300px;
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
    top: 250px;
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
    top: 100px;
    left: 100px;
    z-index: 1;
  }
}
@media screen and (max-width: 375px) {
  h2 {
    font-size: 1.5em;
  }
}
#intro {
  padding-top: 6em;
}
.intro-text {
  border-radius: 10px;
  border: 1px solid #9eadb577;
  box-shadow: 0px 25px 40px rgba(0, 0, 0, 0.2);
}
a {
  color: #455a64;
  border-radius: 30px;
  border: 1px solid #455a64;
  &:hover {
    background-color: #455a64;
    color: white;
  }
}
</style>
