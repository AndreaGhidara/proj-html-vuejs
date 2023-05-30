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
      <img class="artist-shape-2" src="../assets/artist-shape-02.png" alt="">
      <img class="artist-shape-3" src="../assets/artist-shape-03.png" alt="">
      <img class="artist-2" src="../assets/artist-hero-image-02.jpg" alt="">
      <img class="artist-1" src="../assets/artist-hero-image-01.jpg" alt="">
      <img class="artist-3" src="../assets/artist-hero-image-03.png" alt="">
      <img class="artist-4" src="../assets/artist-hero-image-04.jpg" alt="">
      <img class="artist-shape-4" src="../assets/artist-shape-04.png" alt="">
      <img class="artist-shape-1" src="../assets/artist-shape-01.png" alt="">
      <img class="artist-shape-5" src="../assets/artist-shape-05.png" alt="">
      <div class="text-center titleContent">
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

.box {
  height:45rem;
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
  .artist-4{
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
  .titleContent {
    inline-size: 35rem;
    overflow-wrap: break-word;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
  }
}

button {
  background-color: $Orange;


  &:hover {
    background-color: red;
  }
}
</style>
