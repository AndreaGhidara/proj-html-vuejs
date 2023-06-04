<script >

export default {
  nome: "CardEvent",
  components: {
  },
  props: {
    pathImg: String,
    data: String,
    event: String,
    location: String,
  }
}
</script>

<template>
  <div class="d-flex align-items-center py-5">
    <img :src="pathImg" alt="">
    <div class="w-100 cardText ps-4 text-start">
      <p class="data text-secondary fw-semibold">{{data}}</p>
      <p class="event fw-bold">{{event}}</p>
      <p>
        <i class="fa-solid fa-location-arrow"></i>
        {{location}}
      </p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../variables.scss' as *;

.cardCustom {
  width: 300px;
  box-shadow: 5px 5px 15px 5px #cecbcb;
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
