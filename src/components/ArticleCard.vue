<script >

export default {
  nome: "ArticleCard",
  components: {
  },
  props: {
    pathImg: String,
    title: String,
    date: String,
    view: Number,
  }
}
</script>

<template>
  <div class="cardCustom">
    <div class="cardImg">
      <img class="img-fluid" :src="pathImg" alt="">
    </div>
    <div class="caradText bg-white text-start p-3">

      <p class="m-0 pt-3 fw-Medium text-secondary">
        ARTIST
      </p>

      <p class="fw-bold py-1 fs-5">
        {{ title }}
      </p>

      <div class="d-flex justify-content-between pb-5">

        <small class="text-secondary">
          <i class="fa-regular fa-calendar"></i>
          {{ date }}
        </small>

        <small class="text-secondary">
          <i class="fa-regular fa-eye"></i>
          {{ view }}
        </small>

      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../variables.scss' as *;

.cardCustom {
  width: 300px;
  overflow: hidden;
  box-shadow: 5px 5px 15px 5px #cecbcb;
  
  &:hover {
    img{
      transition: all 1s ease-in-out;
      transform: scale(1.1);

      }


    }
  }


.img {
  display: block;
  position: relative;

  .caradText {
    position: absolute;
    bottom: 2rem;
    left: 2rem;
  }
}
</style>
