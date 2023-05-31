<script >
import { Glide, GlideSlide } from 'vue-glide-js'


export default {
  components: {
    nome: "AppTestimonials",
  },
  mounted() {

  }
}
</script>

<template>
  <div class="container py-5">
    <div class="row">
      <div class="col-4">
        <p class="fw-bold">Address</p>
        <p>382 NE 191st ST #87394, MIami, FL 33179-3899</p>
        <p>1+(305)547-9909(9am-5pm EST,monday-friday)</p>
        <p>support@maxcoach.com</p>
        <div>
          social
        </div>
      </div>

      <div class="col-2">
        <p class="fw-bold">Explore</p>
        <ul class="p-0">
          <li>Start here</li>
          <li>Start here</li>
          <li>Start here</li>
          <li>Start here</li>
          <li>Start here</li>
        </ul>
      </div>

      <div class="col-2">
        <p class="fw-bold">
          Explore
        </p>
        <ul class="p-0">
          <li>Start here</li>
          <li>Start here</li>
          <li>Start here</li>
          <li>Start here</li>
          <li>Start here</li>
        </ul>
      </div>

      <div class="col-4">
        <h5>Instagram <span class="cl-primary">@maxcoach</span></h5>

        <div class="row row-cols 3">
          <div class="col">
            <img class="img-fluid"  src="../assets/img/120084500_197897808368764_8114555493043279565_n.jpg" alt="">
          </div>
          <div class="col">
            <img class="img-fluid"  src="../assets/img/120012142_177596140500760_8623485824101406058_n.jpg" alt="">
          </div>
          <div class="col">
            <img class="img-fluid"  src="../assets/img/120099363_364334431619755_7198812647386067017_n.jpg" alt="">
          </div>
        </div>

        
      </div>
    </div>

  </div>
</template>

<style lang="scss" scoped>
  

  ul{
    list-style: none;
  }

  li{
    padding: 0.5rem 0;
    font-size: 14px;
  }
</style>
