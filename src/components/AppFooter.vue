<script >

export default {
  components: {
    nome: "AppTestimonials",
  },
  data() {
    return {
      exploreLink: [
        "Start here",
        "Success story",
        "Blog",
        "Courses",
        "Contact us"
      ],
      informationLink: [
        "Membership",
        "Purchase guide",
        "Privacy policy",
        "Terms of services"
      ],
    }
  },
  mounted() {

  }
}
</script>

<template>
  <div class="container py-5">
    <div class="row">

      <!-- part 1 -->
      <div class="col-4">
        <p class="fw-bold">Address</p>
        <p class="fw-medium">382 NE 191st ST #87394, MIami, FL 33179-3899</p>
        <p class="fw-medium">1+(305)547-9909(9am-5pm EST,monday-friday)</p>
        <p class="fw-medium">support@maxcoach.com</p>
        <div>
          <span class="pe-2 fs-5 text-secondary"><i class="fa-brands fa-facebook-f"></i></span>
          <span class="px-2 fs-5 text-secondary"><i class="fa-brands fa-twitter"></i></span>
          <span class="px-2 fs-5 text-secondary"><i class="fa-brands fa-instagram"></i></span>
          <span class="px-2 fs-5 text-secondary"><i class="fa-brands fa-linkedin-in"></i></span>
        </div>
      </div>

      <!-- part 2 -->
      <div class="col-2">
        <p class="fw-bold">Explore</p>
        <ul class="p-0">
          <template v-for="link in this.exploreLink">
            <li class="fw-semibold">
              <small>
                {{ link }}
              </small>
            </li>
          </template>
        </ul>
      </div>

      <!-- part 3 -->
      <div class="col-2">
        <p class="fw-bold">
          Explore
        </p>
        <ul class="p-0">
          <template v-for="link in this.informationLink">
            <li class="fw-semibold">
              <small>
                {{ link }}
              </small>
            </li>
          </template>
        </ul>
      </div>
      
      <!-- part 4 -->
      <div class="col-4">
        <h5 class="fw-bold">Instagram <small class="tagIg fw-semibold">@maxcoach</small></h5>
        <div class="row row-cols 3">
          <div class="col">
            <img class="img-fluid" src="../assets/img/120084500_197897808368764_8114555493043279565_n.jpg" alt="">
          </div>
          <div class="col">
            <img class="img-fluid" src="../assets/img/120012142_177596140500760_8623485824101406058_n.jpg" alt="">
          </div>
          <div class="col">
            <img class="img-fluid" src="../assets/img/120099363_364334431619755_7198812647386067017_n.jpg" alt="">
          </div>
        </div>
      </div>

    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../variables.scss' as *;

ul {
  list-style: none;
}

li {
  padding: 0.3rem 0;
  font-size: 14px;
}

.tagIg {
  color: $Primary;
}
</style>
