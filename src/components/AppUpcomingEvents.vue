<script >
import CardEvent from './CardEvent.vue';


export default {
  nome: "AppUpcomingEvents",
  components: {
    CardEvent,
  },
  data() {
    return {
      UpEvents: [
        {
          pathImg: "../assets/img/artist-event-04-250x300.jpg",
          data: "NOV, 22, 2020",
          event: "Storytalling Workshop",
          location: "Texas, US",
        },
        {
          pathImg: "../assets/img/artist-event-03-250x300.jpg",
          data: "OCT, 10, 2020",
          event: "Painting Art Contest 2020",
          location: "New York, US",
        },
        {
          pathImg: "../assets/img/artist-event-02-250x300.jpg",
          data: "NOV, 23, 2020",
          event: "International Art Fair 2020",
          location: "Hamburg, Germany",
        },
        {
          pathImg: "../assets/img/artist-event-01-250x300.jpg",
          data: "DEC, 15, 2020",
          event: "Street Performance: Call for Artist",
          location: "Illinois, US",
        },
      ]

    }
  },
  methods: {
    getImagePath: function (imgPath) {
      return new URL(imgPath, import.meta.url).href;
    }
  },
  mounted() {

  }
}
</script>

<template>
  <div class="box">
    <div class="container text-center">
      <div class="py-5">
        <h2 class="artist">Upcoming Events</h2>
        <h2>Let's Work Together</h2>
      </div>

      <div class="container">
        <div class="row row-cols-2">
          <CardEvent :pathImg="this.getImagePath(this.UpEvents[0].pathImg)" :data="this.UpEvents[0].data"
            :event="this.UpEvents[0].event" :location="this.UpEvents[0].location" />
          <CardEvent :pathImg="this.getImagePath(this.UpEvents[1].pathImg)" :data="this.UpEvents[1].data"
            :event="this.UpEvents[1].event" :location="this.UpEvents[1].location" />
          <CardEvent class="flex-row-reverse" :pathImg="this.getImagePath(this.UpEvents[2].pathImg)"
            :data="this.UpEvents[2].data" :event="this.UpEvents[2].event" :location="this.UpEvents[2].location" />
          <CardEvent class="flex-row-reverse" :pathImg="this.getImagePath(this.UpEvents[3].pathImg)"
            :data="this.UpEvents[3].data" :event="this.UpEvents[3].event" :location="this.UpEvents[3].location" />
        </div>
      </div>

    </div>
    <div class="sideTitle">
      <h1 class="title SectionTitle m-0">Events</h1>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../variables.scss' as *;

.box {
  position: relative;
}

.card-custom {
  width: 400px;
}

.sideTitle {
  position: absolute;
  left: -10%;
  top: 50%;

  .title {
    font-size: 180px;
    line-height: 0.9em;
    -webkit-text-stroke-color: #F4EBE2;
    -webkit-text-fill-color: rgba(0, 0, 0, 0);
    -webkit-text-stroke-width: 1px;
    transform: rotate(90deg);
  }
}</style>
