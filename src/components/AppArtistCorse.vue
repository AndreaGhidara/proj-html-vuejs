<script >
import CardCourse from './CardCourse.vue';
import ButtonCustom from './ButtonCustom.vue';

export default {
  nome: "AppArtistCorse",
  components: {
    CardCourse,
    ButtonCustom
  },
  data() {
    return {
      courses: [
        {
          imgPath: "../assets/img/artist-course-08-480x480.jpg",
          price: 18.80,
          title: "The Acrylic Painting Accademy",
          lessons: 4,
          students: 50,
        },
        {
          imgPath: "../assets/img/artist-course-07-480x480.jpg",
          price: 21.00,
          title: "Drawing and Shading: Complete Course",
          lessons: 14,
          students: 50,
        },
        {
          imgPath: "../assets/img/artist-course-06-480x480.jpg",
          price: 19.80,
          title: "The Color Theory for Digital Artist",
          lessons: 7,
          students: 50,
        },
        {
          imgPath: "../assets/img/artist-course-05-480x480.jpg",
          price: 35.00,
          title: "Ultimate Guide to Digital Sketching for Beginner",
          lessons: 14,
          students: 50,
        },
        {
          imgPath: "../assets/img/artist-course-04-480x480.jpg",
          price: 19.00,
          title: "Portait Drawing The Smart Way",
          lessons: 2,
          students: 50,
        },
        {
          imgPath: "../assets/img/artist-course-03-480x480.jpg",
          price: 19.00,
          title: "Mastering Watercolor Painting from Beginner",
          lessons: 9,
          students: 50,
        },
        {
          imgPath: "../assets/img/artist-course-02-480x480.jpg",
          price: 18.80,
          title: "The Art & Science of Drawing",
          lessons: 4,
          students: 50,
        },
        {
          imgPath: "../assets/img/artist-course-01-480x480.jpg",
          price: 22.00,
          title: "The Colored Pencil Drawing Course",
          lessons: 4,
          students: 50,
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
  <div class="text-center py-5">
    <h2 class="artist">Artist Coaching</h2>
    <h2>Latest Online Courses</h2>
    <div class="pt-3">
      <div class="container">
        <div class="row row-cols-4">
          <div v-for="course in this.courses" class="col">
            <CardCourse :imgPath=this.getImagePath(course.imgPath) :prezzo="Number(course.price).toFixed(2)" :titolo="course.title" :lezioni=course.lessons
              :studenti=course.students />
          </div>
        </div>
      </div>
      <div>
        <ButtonCustom class="px-5" text="View All courses &#8594;" />
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
$Orange: #Ef6F31;
$Sky: #6AC5F1;

button {
  background-color: #fdf0ea;
  color: $Orange;

  &:hover {
    background-color: $Sky;
  }
}
</style>
