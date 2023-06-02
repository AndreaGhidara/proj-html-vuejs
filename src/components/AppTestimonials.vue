<script >
import { Splide, SplideSlide } from '@splidejs/vue-splide';
import Carousel from './Carousel.vue';


export default {
  nome: "AppTestimonials",
  components: {
    Splide,
    SplideSlide,
    Carousel
  },
  data() {
    return {
      testimonials: [
        {
          title: "High level of efficiency and scientific teaching methods",
          review: "I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.",
          profilePath: "https://maxcoach.thememove.com/main/wp-content/uploads/sites/1/2020/05/artist-testimonial-avatar-04.jpg",
          name: "Mina Hollace",
          job: "/ Freelancer",
        },
        {
          title: "Professional team of specialists and passionate mentors at reach ",
          review: "I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.",
          profilePath: "https://maxcoach.thememove.com/main/wp-content/uploads/sites/1/2020/05/artist-testimonial-avatar-04.jpg",
          name: "Madley Pondor",
          job: "/ IT Specialist",
        },
        {
          title: "The MaxCoach team works really hard to ensure high quality",
          review: "I am happy with their arrangement of lessons and subjects. They reflect a scientific  investigation into effective methods to be adopted for learners of all levels.",
          profilePath: "https://maxcoach.thememove.com/main/wp-content/uploads/sites/1/2020/05/artist-testimonial-avatar-04.jpg",
          name: "Luvic Dubble",
          job: "/ Private Tutor",
        },
        {
          title: "It's a choice of quality for people with special needs",
          review: "I'm a very strict person so I require everything to be organized and neat. Then, I'll be able to make things right and shine. MaxCoach guys just got me.",
          profilePath: "https://maxcoach.thememove.com/main/wp-content/uploads/sites/1/2020/05/artist-testimonial-avatar-04.jpg",
          name: "Florence Themes",
          job: "/ Multimedia Admin",
        },
      ]
    }
  },
  setup() {
    const options = {
      rewind: true,
      gap: '1rem',
    }

    return { options }
  },
  mounted() {

  },
}
</script>

<template>
  <div class="text-center box p-5">
    <h2 class="artist">Testimonials</h2>
    <h2>Why do people love me?</h2>
    <div>
      <Carousel />
      <!-- <div class="w-100 d-flex">
        <div class="bg-white testimonialsCard text-start p-5 m-2">
          <h5 class="fw-bold">{{ this.testimonials[0].title }}</h5>
          <p>{{ this.testimonials[0].review }}</p>
          <div class="d-flex align-items-center">
            <img :src="this.testimonials[0].profilePath" alt="">
            <div class="w-100 text-start ps-3">
              <p class="fw-bold">Nome: </p>
              <p class="text-secondary">/ freelencer </p>
            </div>
          </div>
        </div>
        <div class="bg-white testimonialsCard text-start p-5 m-2">
          <h5 class="fw-bold">{{ this.testimonials[0].title }}</h5>
          <p>{{ this.testimonials[0].review }}</p>
          <div class="d-flex align-items-center">
            <img :src="this.testimonials[0].profilePath" alt="">
            <div class="w-100 text-start ps-3">
              <p class="fw-bold">Nome: </p>
              <p class="text-secondary">/ freelencer </p>
            </div>
          </div>
        </div>
        <div class="bg-white testimonialsCard text-start p-5 m-2">
          <h5 class="fw-bold">{{ this.testimonials[0].title }}</h5>
          <p>{{ this.testimonials[0].review }}</p>
          <div class="d-flex align-items-center">
            <img :src="this.testimonials[0].profilePath" alt="">
            <div class="w-100 text-start ps-3">
              <p class="fw-bold">Nome: </p>
              <p class="text-secondary">/ freelencer </p>
            </div>
          </div>
        </div>
      </div> -->
      
    </div>
  </div>
</template>

<style lang="scss" scoped>
img {
  width: 100px;
  border-radius: 50%;
}

.testimonialsCard {
  width: calc(100% / 3);
}

.box {
  background-color: #faf8f6;

}
</style>
