<template>
  <!-- HEADER -->
  <div class="container-fluid">
    <h1 class="text-uppercase font-weight-lighter">
      Magalhaes Florian
      <span class="d-block h5 font-weight-bold">{{ subtitle }}</span>
    </h1>
  </div>
  <!-- END HEADER -->
</template>

<script>
export default {
  name: "Header",
  data: () => {
    return {
      subtitle: " ",
      i: 0,
    };
  },
  methods: {
    writingSubtitle() {
      //Animation like keyboard writing
      let subtitle = "Développeur Web & Mobile";
      let speed = 100;

      if (this.i < subtitle.length) {
        this.subtitle += subtitle.charAt(this.i);
        this.i++;
        setTimeout(this.writingSubtitle, speed);
      } else {
        this.i = 1;
        setTimeout(() => (this.subtitle = "D"), 5000);
        setTimeout(this.writingSubtitle, 5000);
      }
    },
  },
  created() {
    this.writingSubtitle();
  },
};
</script>

<style scoped lang="scss">
.container-fluid {
  padding-top: 8em;
}
</style>
