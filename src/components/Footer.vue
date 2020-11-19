<template>
  <section id="footer" class="pt-3">
    <div class="container-fluid">
      <p class="mb-0">
        Copyright © 2020 Tous droits réservés | Florian Magalhaes
      </p>
    </div>
  </section>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped lang="scss">
#footer {
  background-color: #455a64;
  color: white;
  font-size: 0.8em;
  @media screen and (max-width: 374px) {
    font-size: 0.6em;
  }
}
</style>
