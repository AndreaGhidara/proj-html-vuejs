<script >

export default {
  components: {
    nome: "AppAritclesAndTips",

  },
  mounted() {

  }
}
</script>

<template>
  <div class="container-fluid back text-center">
    <h2 class="artist">Aritcles And Tips</h2>
    <h2 class="pb-4">Latest from the Blog</h2>
    <div class="d-flex justify-content-center">

      <div class="d-flex align-items-center p-5">
        <div class="cardCustom">
          <div class="cardImg">
            <img class="img-fluid" src="../assets/img/artist-blog-03-480x356.jpeg" alt="">
          </div>
          <div class="caradText bg-white text-start ps-3">
            <p class="m-0 pt-3">Artist</p>
            <p>
              <strong>
                Brush Sronkes Energize Trees in Paintings
              </strong>
            </p>
            <p class="d-flex justify-content-between">
              <span>May 15,20</span>
              <span>688 views</span>
            </p>
          </div>
        </div>
  
      </div>

      <div class="p-3 img text-white">
        <img class="img-fluid" src="../assets/img/artist-blog-02-500x680.jpg" alt="">
        <div class="caradText text-start ps-3 ">
            <p class="m-0 pt-3 fs-5">Artist</p>
            <p>
              <strong class="fs-3">
                Connection Beetween Self-Partaits and Identity
              </strong>
            </p>
            <p >
              <span>May 15,20</span>
              <span class="ps-4">688 views</span>
            </p>
          </div>
      </div>

      <div class="d-flex p-5">
        <div class="cardCustom">
          <div class="cardImg">
            <img class="img-fluid" src="../assets/img/artist-blog-01-480x356.jpg" alt="">
          </div>
          <div class="caradText bg-white text-start ps-3">
            <p class="m-0 pt-3">Artist</p>
            <p>
              <strong>
                Brush Sronkes Energize Trees in Paintings
              </strong>
            </p>
            <p class="d-flex justify-content-between">
              <span>May 15,20</span>
              <span>688 views</span>
            </p>
          </div>
        </div>
  
      </div>

    </div>
    <div class="py-5">
      <p>Get into details now? View all posts &#8594;</p>
    </div>

  </div>
</template>

<style lang="scss" scoped>
$Orange: #Ef6F31;

.cardCustom {
  width: 300px;
}

.img{
  display: block;
  position: relative;

  .caradText{
    position: absolute;
    bottom: 2rem;
    left: 2rem;
  }
}

.back{
  background-image: url("../assets/img/maxcoach-shape-03.png"),url(../assets/img/maxcoach-shape-12.png) ;
  background-repeat: no-repeat,no-repeat;
  background-position: 40% 40%, 39% 16%;
}
</style>
