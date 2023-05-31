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
        <div class="col d-flex justify-content-end align-items-center">
          <img class="artist-1 " src="../assets/img/artist-hero-image-01.jpg" alt="">
          <img class="artist-2 " src="../assets/img/artist-hero-image-02.jpg" alt="">
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
        <div class="col d-flex align-items-end">
          <img class="artist-4 pb-5" src="../assets/img/artist-hero-image-04.jpg" alt="">
        </div>
      </div>
    </div>

</template>

<style lang="scss" scoped>

$Orange: #Ef6F31;
$Sky: #6AC5F1;

button{
  background-color: $Orange;

  &:hover{
            background-color: $Sky;
        }
}
.customBg {
  background-color: #fbf9f6;
  position: relative;
  height: 800px;
  background-image: url(../assets/img/artist-shape-01.png), url(../assets/img/artist-shape-02.png), url(../assets/img/artist-shape-03.png), url(../assets/img/artist-shape-04.png), url(../assets/img/artist-shape-05.png), url(../assets/img/artist-hero-image-03.png), ;
  background-repeat: no-repeat, no-repeat, no-repeat, no-repeat, no-repeat, no-repeat;
  background-position: 81% 0%, 0% 0%, 0% 80%, 87% 30%, 90% 100%, 29% 100%,;
  .artist-1 {
    position: relative;
    z-index: 1;
    transform: translate(5%, 90%);
  }

  .artist-2 {
    transform: translateY(-15%);
  }
}

</style>
