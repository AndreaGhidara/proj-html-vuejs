<script >
import { Glide, GlideSlide } from 'vue-glide-js'


export default {
  components: {
    nome: "AppTestimonials",
    [Glide.name]: Glide,
    [GlideSlide.name]: GlideSlide
  },
  mounted() {

  }
}
</script>

<template>
  <div class="text-center">
    <h2 class="artist">Testimonials</h2>
    <h2>Why do people love me?</h2>
    <div>

      <div>
        SLIDER
      </div>

    </div>
  </div>
</template>

<style lang="scss" scoped>
div {
  background-color: lightcoral;
}

.box {
  position: relative;


  .coaching-shape-05 {
    position: absolute;
    top: -2rem;
    left: -2rem;
    z-index: -1;
  }

  .coaching-shape-12 {
    position: absolute;
    bottom: -1rem;
    right: -7rem;
    z-index: -1;
  }
}
</style>
