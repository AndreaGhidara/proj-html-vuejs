<script >
import ArticleCard from './ArticleCard.vue';
import Carousel from './Carousel.vue';




export default {
  components: {
    nome: "AppAritclesAndTips",
    ArticleCard,
    Carousel,
},
  data() {
    return {
      articles: [
        {
          imgPath: "../assets/img/artist-blog-03-480x356.jpeg",
          title:"Brush Sronkes Energize Trees in Paintings",
          date: "may 15,2020",
          view: 688,
        },
        {
          imgPath: "../assets/img/artist-blog-01-480x356.jpg",
          title: "Brush Sronkes Energize Trees in Paintings",
          date: "May 15,20",
          view: 603,
        },
      ]
    }
  },
  methods: {
    getImagePath: function (imgPath) {
      return new URL(imgPath, import.meta.url).href;
    }
  }

}
</script>

<template>
  

  <div class="container-fluid back p-5 text-center">
    <h2 class="artist">Aritcles And Tips</h2>
    <h2 class="pb-4">Latest from the Blog</h2>
    <div class="d-flex justify-content-center">

      <!-- Article 1 -->
      <div class="d-flex align-items-center p-5">
        <ArticleCard :pathImg="getImagePath(this.articles[0].imgPath)" :title="this.articles[0].title" :date="this.articles[0].date" :view="this.articles[0].view"/>
      </div>
      <!-- Article 2 -->
      <div class="p-3 CardContainer text-white">
        <img class="img-fluid" src="../assets/img/artist-blog-02-500x680.jpg" alt="">
        
        <div class="caradText text-start  ">
          <div>
            <p class="m-0 pt-3 fw-Medium  text-white fs-5">Artist</p>
            <p class="fs-3 fw-bold">
                Connection Beetween Self-Partaits and Identity
            </p>
          </div>
          <div class="d-flex pb-5">
              <small>
                <i class="fa-regular fa-calendar"></i>
                May 15,20
              </small>
              <small class="ps-4">
                <i class="fa-regular fa-eye"></i>
                688 views
              </small>
          </div>
        </div>
      </div>
      <!-- Article 3 -->
      <div class="d-flex align-items-start p-5">
        <ArticleCard :pathImg="getImagePath(this.articles[1].imgPath)" :title="this.articles[1].title" :date="this.articles[1].date" :view="this.articles[1].view"/>
      </div>

    </div>
    <!-- info -->
    <div class="py-5">
      <p>
        Get into details now? 
        <strong class="border-bottom">View all posts <i class="fa-solid fa-arrow-right-long"></i></strong> 
      </p>
    </div>

  </div>
</template>

<style lang="scss" scoped>
$Orange: #Ef6F31;

img{
  // filter: invert(50%) sepia(50%) saturate(0%) hue-rotate(0deg) brightness(50%) contrast(100%);
  filter:brightness(90%) ;
  box-shadow: 5px 5px 15px 5px #cecbcb;
}

strong{
  color: $Orange;
}

.CardContainer{
  display: block;
  position: relative;

  .caradText{
    padding: 2rem;
    position: absolute;
    bottom: 0;
  }
}

.back{
  background-color: #f5f7fa;
  background-image: url("../assets/img/maxcoach-shape-03.png"),url(../assets/img/maxcoach-shape-12.png) ;
  background-repeat: no-repeat,no-repeat;
  background-position: 40% 40%, 39% 16%;
}
</style>
