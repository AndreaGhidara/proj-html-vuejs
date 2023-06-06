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
  <div class="d-flex align-items-center py-5 overflow-hidden">
    <div class="img-Container">
      <img class="img-fluid" :src="pathImg" alt="">
    </div>
    <div class="w-100 cardText ps-4 text-start">
      <p class="data text-secondary fw-semibold">{{ data }}</p>
      <p class="event fw-bold">{{ event }}</p>
      <p>
        <i class="fa-solid fa-location-arrow"></i>
        {{ location }}
      </p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../variables.scss' as *;

.img-Container{
  width: 430px;
  overflow: hidden;
}

img {
  box-shadow: 5px 5px 15px 5px #cecbcb;
  transition: all 1s ease-in-out;
  &:hover {
    transform: scale(1.1);
    

  }
}


</style>
