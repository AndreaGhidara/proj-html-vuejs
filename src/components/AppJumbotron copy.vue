<script >

export default {
  components: {
    nome: "AppJumbotron"
  }
}
</script>

<template>
  <div class="container-fluid  box p-0">
    <div class="mini-box h-100">
      <img class="artist-shape-2" src="../assets/img/artist-shape-02.png" alt="">
      <img class="artist-shape-3" src="../assets/img/artist-shape-03.png" alt="">
      <img class="artist-2" src="../assets/img/artist-hero-image-02.jpg" alt="">
      <img class="artist-1" src="../assets/img/artist-hero-image-01.jpg" alt="">
      <img class="artist-3" src="../assets/img/artist-hero-image-03.png" alt="">
      <img class="artist-4" src="../assets/img/artist-hero-image-04.jpg" alt="">
      <img class="artist-shape-4" src="../assets/img/artist-shape-04.png" alt="">
      <img class="artist-shape-1" src="../assets/img/artist-shape-01.png" alt="">
      <img class="artist-shape-5" src="../assets/img/artist-shape-05.png" alt="">
      <div class="shape">
        <svg xmlns="http://www.w3.org/2000/svg" version="1.1" width="480px" height="480px" viewBox="0 0 200 202">
          <path class="element-svg-1"
            d="M139.374493,198.087515 C155.702187,206.99353 190.724846,197.001323 197.677982,159.049528 C204.827153,120.027728 184.496324,118.997566 188.045232,104.801934 C202.287755,83.6528313 204.827153,56.662651 190.073179,40.4146034 C153.570125,2.39058926 144.444362,48.0194062 114.025151,20.1351292 C101.727304,7.83728238 83.0989526,-6.73517414 56.2286492,3.40456297 C18.2385839,17.7404371 27.3303985,47.659333 27.3303985,69.3128542 C27.3303985,76.9370868 3.11408002,91.2696589 0.460095291,110.885776 C-2.88628833,135.619549 12.6277797,168.175291 27.3303985,179.329002 C50.6517938,205.692318 86.6478605,199.608476 102.87144,190.482713 C116.802125,182.646702 128.220783,192.003673 139.374493,198.087515 Z">
          </path>
        </svg>
      </div>

      <div class="text-center titleContent">
        <h2 class="artist">Hello, Im Martin</h2>
        <h2>
          <strong>
            Artist Coaching And Mentoring Might Be for You
          </strong>
        </h2>
        <button class="btn text-white">
          <strong>Get started today</strong>
        </button>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
$Orange: #Ef6F31;
$Sky: #6AC5F1;
$LightGray: #F5F5F5;
$Black: #333333;
$White:#ffffff;
$BluRoyale: #1972F5;


.box {
  height: 45rem;
  background-color: rgb(214, 218, 219);
}

.mini-box {
  position: relative;

  .artist-shape-3 {
    position: absolute;
    left: 0;
    top: 10rem;
  }

  .artist-shape-2 {
    position: absolute;
    top: 0;
    left: -3rem;
  }

  .artist-1 {
    position: absolute;
    bottom: 3rem;
    left: 9rem;
  }

  .artist-2 {
    position: absolute;
    top: 6rem;
    left: 21rem;
    z-index: 1;
  }

  .artist-3 {
    position: absolute;
    z-index: 0;
    bottom: 1rem;
    left: 30rem;
  }

  .artist-4 {
    width: 20rem;
    position: absolute;
    bottom: 4rem;
    right: 20rem;
    z-index: 1;
  }

  .artist-shape-1 {
    position: absolute;
    top: 0;
    right: 10rem;
  }

  .artist-shape-4 {
    height: 20rem;
    rotate: 10deg;
    position: absolute;
    top: 4rem;
    right: 13rem;
    z-index: 0;
  }

  .artist-shape-5 {
    position: absolute;
    bottom: 0rem;
    right: 11rem;
    z-index: 0;
  }

  // TODO controllare la posizione
  .element-svg-1{
    fill: #B2E0F6;
    position: absolute;
    bottom: 0;
  }

  .titleContent {
    inline-size: 35rem;
    overflow-wrap: break-word;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
}

button {
  background-color: $Orange;


  &:hover {
    background-color: red;
  }
}</style>
