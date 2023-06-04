<script >

export default {
  components: {
    nome: "AppCoachingVideo"
  }
}
</script>

<template>
  <div class="d-flex justify-content-center align-items-center my-5 py-5 box">
    <div class="imgContainer">
      <img class="img" src="../assets/img/artist-video-poster.jpg" alt="">
      <div class="svgBox">
        <svg xmlns="http://www.w3.org/2000/svg" version="1.1" width="200px" height="202px" viewBox="0 0 200 202">
          <path class="shape-fill"
            d="M139.374493,198.087515 C155.702187,206.99353 190.724846,197.001323 197.677982,159.049528 C204.827153,120.027728 184.496324,118.997566 188.045232,104.801934 C202.287755,83.6528313 204.827153,56.662651 190.073179,40.4146034 C153.570125,2.39058926 144.444362,48.0194062 114.025151,20.1351292 C101.727304,7.83728238 83.0989526,-6.73517414 56.2286492,3.40456297 C18.2385839,17.7404371 27.3303985,47.659333 27.3303985,69.3128542 C27.3303985,76.9370868 3.11408002,91.2696589 0.460095291,110.885776 C-2.88628833,135.619549 12.6277797,168.175291 27.3303985,179.329002 C50.6517938,205.692318 86.6478605,199.608476 102.87144,190.482713 C116.802125,182.646702 128.220783,192.003673 139.374493,198.087515 Z">
          </path>
        </svg>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>

svg{
  width: 100%;
  height: auto;
}

.box {
  background-image: url(../assets/img/maxcoach-shape-12.png), url(../assets/img/maxcoach-shape-05.png);
  background-repeat: no-repeat, no-repeat;
  background-position: 80% 93%, 24% 5%;
}

.imgContainer{
  position: relative;
}
.shape-fill {
  fill: #B2E0F6;
}

.svgBox {
  position: absolute;
  z-index: -1;
  top: -3rem;
  left: -5rem;
  width: 226px;
  transform: rotate(0deg) scale(1, 1);
  color: #B2E0F6;
}

</style>

970 * 570