<script >

export default {
  components: {
    nome: "AppUpcomingEvents",

  },
  mounted() {

  }
}
</script>

<template>
  <div>
    <div class="container text-center">
      <div class="pb-5">
        <h2 class="artist">Upcoming Events</h2>
        <h2>Let's Work Together</h2>
      </div>
      
      <div class="container">
        <div class="row row-cols-2">
          <div class="col d-flex align-items-center py-5">
            <img src="../assets/img/artist-event-04-250x300.jpg" alt="">
            <div class="w-100 cardText ps-4 text-start">
              <p>Nov, 22, 2020</p>
              <p>Storytalling Workshop</p>
              <p>test</p>
            </div>
          </div>
          <div class="col d-flex align-items-center py-5">
            <img src="../assets/img/artist-event-03-250x300.jpg" alt="">
            <div class="w-100 cardText ps-4 text-start">
              <p>Nov, 22, 2020</p>
              <p>Storytalling Workshop</p>
              <p>test</p>
            </div>
          </div>
          <div class="col d-flex align-items-center py-5">
            <img class="order-1" src="../assets/img/artist-event-02-250x300.jpg" alt="">
            <div class="w-100 cardText ps-4 text-start">
              <p>Nov, 22, 2020</p>
              <p>Storytalling Workshop</p>
              <p>test</p>
            </div>
          </div>
          <div class="col d-flex align-items-center py-5">
            <img class="order-1" src="../assets/img/artist-event-01-250x300.jpg" alt="">
            <div class="w-100 cardText ps-4 text-start">
              <p>Nov, 22, 2020</p>
              <p>Storytalling Workshop</p>
              <p>test</p>
            </div>
          </div>
        </div>
      </div>
        
    </div>
  </div>
</template>

<style lang="scss" scoped>
$Orange: #Ef6F31;

.card-custom{
  width: 400px;

}


</style>
