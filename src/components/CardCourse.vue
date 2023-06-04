<script >

export default {
  nome: "CardCourse",
  components: {

  },
  props: {
    imgPath: String,
    prezzo: Number,
    titolo: String,
    lezioni: Number,
    studenti: Number,
  },

}
</script>

<template>
  <div class="cardCustom py-2">
    <div class="cardImg">
      <img class="img-fluid" :src="imgPath" alt="">
    </div>
    <div class="caradText d-flex flex-column justify-content-around text-start ps-3">
      <div>
        <p class="price m-0">$ {{ prezzo }}</p>
      </div>
      <div>
        <p class="title m-0">{{ titolo }}</p>
      </div>
      <div class="d-flex justify-content-between">
        <p>
          <i class="fa-regular fa-file-lines"></i>
          {{ lezioni }} Lessons
        </p>
        <p>
          <i class="fa-solid fa-people-group"></i>
          {{ studenti }} Students
        </p>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../variables.scss' as *;

.cardCustom {
  height: 500px;
  overflow: hidden;
  
  &:hover {
      .caradText {
        transform: translateY(-50px);
        border: 1px solid #Ef6F31;
      }
    }
  .cardImg{
    transition: transform .5s ease;

    &:hover{
      transform: scale(1.3);
      
    }
    
  }
}

  .caradText {
    height: 150px;
    background-color: white;

    .title {
      font-size: larger;
      font-weight: 600;

      &:hover {
        color: #Ef6F31;
      }
    }

    .price {
      color: #Ef6F31;
      font-weight: 800;
    }

  }

</style>
