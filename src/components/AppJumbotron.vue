<script >
import ButtonCustom from './ButtonCustom.vue';

export default {
  nome: "AppJumbotron",

  components: {
    ButtonCustom,
  }
}
</script>

<template>
  <div class="container-full customBg d-flex flex-column justify-content-center align-items-center">
    <div class="row row-cols-3 w-100 h-100">
      <div class="col d-flex justify-content-end align-items-center left">
        <img class="artist-1 " src="../assets/img/artist-hero-image-01.jpg" alt="">
        <img class="artist-2 " src="../assets/img/artist-hero-image-02.jpg" alt="">
        <div class="shape">
          <svg xmlns="http://www.w3.org/2000/svg" version="1.1" width="200px" height="202px" viewBox="0 0 200 202">
            <path class="shape-fill"
              d="M139.374493,198.087515 C155.702187,206.99353 190.724846,197.001323 197.677982,159.049528 C204.827153,120.027728 184.496324,118.997566 188.045232,104.801934 C202.287755,83.6528313 204.827153,56.662651 190.073179,40.4146034 C153.570125,2.39058926 144.444362,48.0194062 114.025151,20.1351292 C101.727304,7.83728238 83.0989526,-6.73517414 56.2286492,3.40456297 C18.2385839,17.7404371 27.3303985,47.659333 27.3303985,69.3128542 C27.3303985,76.9370868 3.11408002,91.2696589 0.460095291,110.885776 C-2.88628833,135.619549 12.6277797,168.175291 27.3303985,179.329002 C50.6517938,205.692318 86.6478605,199.608476 102.87144,190.482713 C116.802125,182.646702 128.220783,192.003673 139.374493,198.087515 Z">
            </path>
          </svg>
        </div>
        <div class="shapeDots">
          <img class="" src="../assets/img/artist-shape-03.png" alt="">
        </div>
      </div>
      <div class="col d-flex flex-column justify-content-center text-center">
        <h2 class="artist">Hello, Im Martin</h2>
        <h2 class="fw-bold titleContent">
          Artist Coaching And Mentoring Might Be for You
        </h2>
        <div class="text-center">
          <ButtonCustom class="text-white" text="Get started today" />
        </div>
      </div>
      <div class="col d-flex align-items-end right">
        <img class="artist-4 pb-5" src="../assets/img/artist-hero-image-04.jpg" alt="">
        <div class="shapeYellow">
          <svg xmlns="http://www.w3.org/2000/svg" version="1.1" width="200px" height="202px" viewBox="0 0 200 202">
            <path class="elementor-shape-fill"
              d="M139.374493,198.087515 C155.702187,206.99353 190.724846,197.001323 197.677982,159.049528 C204.827153,120.027728 184.496324,118.997566 188.045232,104.801934 C202.287755,83.6528313 204.827153,56.662651 190.073179,40.4146034 C153.570125,2.39058926 144.444362,48.0194062 114.025151,20.1351292 C101.727304,7.83728238 83.0989526,-6.73517414 56.2286492,3.40456297 C18.2385839,17.7404371 27.3303985,47.659333 27.3303985,69.3128542 C27.3303985,76.9370868 3.11408002,91.2696589 0.460095291,110.885776 C-2.88628833,135.619549 12.6277797,168.175291 27.3303985,179.329002 C50.6517938,205.692318 86.6478605,199.608476 102.87144,190.482713 C116.802125,182.646702 128.220783,192.003673 139.374493,198.087515 Z">
            </path>
          </svg>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../variables.scss' as *;

button {
  background-color: $Primary;

  &:hover {
    background-color: $Sky;
  }
}


.left {
  position: relative;
  .shape {
    position: absolute;
    bottom: 2rem;
    left: -4rem;
    width: 478px;
    transform: rotate(0deg) scale(1, 1);
    fill: #B2E0F6;
    z-index: 0;
  
    svg {
      width: 100%;
      height: auto;
    }
  }
  
  .shape-fill {
    position: absolute;
  }
  
  .shapeDots {
    position: absolute;
    left: 0;
    bottom: 10%;
  }
}

.right{
  position: relative;
  
  .artist-4{
    z-index: 1;
  }
  .shapeYellow{
    position: absolute;
    fill: #FFCD00;
    z-index: 0;
    left: -3rem;
  }
}


.customBg {
  background-color: #fbf9f6;
  position: relative;
  height: 800px;
  background-image: url(../assets/img/artist-shape-01.png), url(../assets/img/artist-shape-02.png), url(../assets/img/artist-shape-04.png), url(../assets/img/artist-shape-05.png), url(../assets/img/artist-hero-image-03.png), ;
  background-repeat: no-repeat, no-repeat, no-repeat, no-repeat, no-repeat;
  background-position: 81% 0%, 0% 0%, 87% 30%, 90% 100%, 29% 100%, ;

  .artist-1 {
    position: relative;
    z-index: 2;
    transform: translate(5%, 90%);
  }

  .artist-2 {
    z-index: 1;
    transform: translateY(-15%);
  }
}
</style>
