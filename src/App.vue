<script>
import { store } from './data/store';

import AppNavbar from './components/AppNavbar.vue';
import AppCounter from './components/AppCounter.vue';
import AppJumbotron from './components/AppJumbotron.vue';
import AppCoaching from './components/AppCoaching.vue';
import AppCoachingNote from './components/AppCoachingNote.vue';
import AppCoachingVideo from './components/AppCoachingVideo.vue';
import AppTestimonials from './components/AppTestimonials.vue';
import AppArtistCorse from './components/AppArtistCorse.vue';
import AppAritclesAndTips from './components/AppAritclesAndTips.vue'
import AppUpcomingEvents from './components/AppUpcomingEvents.vue';
import AppNewsLetter from './components/AppNewsLetter.vue';
import AppFooter from './components/AppFooter.vue';




export default {
  components:{
    AppCounter,
    AppNavbar,
    AppJumbotron,
    AppCoaching,
    AppCoachingNote,
    AppCoachingVideo,
    AppTestimonials,
    AppArtistCorse,
    AppAritclesAndTips,
    AppUpcomingEvents,
    AppNewsLetter,
    AppFooter
},
  data(){

  },
  methods:{

  },
  mounted(){

  }
}


</script>

<template>
  <section id="header">
    <AppCounter />
    <AppNavbar />
    <AppJumbotron />
  </section>
  <!-- ArtistCoaching -->
  <AppCoaching />
  <AppCoachingNote />
  <AppCoachingVideo />
  <!-- Testimonials -->
  <AppTestimonials />
  <!-- ArtistCorse -->
  <AppArtistCorse />
  <!-- Articoles and Tips -->
  <AppAritclesAndTips />
  <!-- UpcomingEvents -->
  <AppUpcomingEvents />
  <!-- NewsLetter -->
  <AppNewsLetter />
  <!-- Footer -->
  <AppFooter />
  <!-- Copyright -->
</template>

<style lang="scss" scoped>

</style>
