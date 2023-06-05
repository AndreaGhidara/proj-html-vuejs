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
    <div class="elementor-shape">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
        <path fill="#faf8f6" fill-opacity="0.97"
          d="M0,288L30,250.7C60,213,120,139,180,112C240,85,300,107,360,138.7C420,171,480,213,540,229.3C600,245,660,235,720,213.3C780,192,840,160,900,149.3C960,139,1020,149,1080,181.3C1140,213,1200,267,1260,266.7C1320,267,1380,213,1410,186.7L1440,160L1440,320L1410,320C1380,320,1320,320,1260,320C1200,320,1140,320,1080,320C1020,320,960,320,900,320C840,320,780,320,720,320C660,320,600,320,540,320C480,320,420,320,360,320C300,320,240,320,180,320C120,320,60,320,30,320L0,320Z">
        </path>
      </svg>
    </div>
  </div>
</template>

<style lang="scss" scoped>
svg {
  width: 100%;
  height: auto;
}


.box {
  position: relative;
  background-image: url(../assets/img/maxcoach-shape-12.png), url(../assets/img/maxcoach-shape-05.png);
  background-repeat: no-repeat, no-repeat;
  background-position: 80% 93%, 24% 5%;
  .elementor-shape {
    position: absolute;
    z-index: -1;
    transform: scaleX(-1);
    bottom: -8rem;
    width: 100%;
    height: 500px;
    
  }
}

.imgContainer {
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