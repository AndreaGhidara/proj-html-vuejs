<script >

export default {
  nome: "AppNavbar",
  components: {

  },
  data() {
    return {
      navLink: ["Home", "Pages", "Courses", "Features", "Blog", "Shop",],
    }
  },
  methods: {

  },
  mounted() {

  }
}
</script>

<template>
  <nav class="bg-white">
    <div class="container d-flex justify-content-between align-items-center py-4 px-0">
      <div>
        <img style="width: 10rem;" src="/dark-logo.png" alt="">
      </div>
      <div>
        <ul class="d-flex m-0">
          <li v-for="links in navLink">
            {{ links }}
            <i class="fa-solid fa-angle-down"></i>
          </li>
        </ul>
      </div>
      <div>
        <span><i class="fa-brands fa-facebook-f"></i></span>
        <span><i class="fa-brands fa-twitter"></i></span>
        <span><i class="fa-brands fa-instagram"></i></span>
        <span><i class="fa-brands fa-linkedin-in"></i></span>
      </div>
    </div>
  </nav>
  <div class="d-flex flex-column align-items-center navLateral bg-white rounded py-2">
    <span>
      <i class="py-2 fa-solid fa-ruler-combined"></i>
    </span>
    <span>
      <i class="py-2 fa-solid fa-life-ring"></i>
    </span>
    <span>
      <i class="py-2 fa-solid fa-book"></i>
    </span>
    <span>
      <i class="py-2 fa-solid fa-cart-shopping"></i>
    </span>
  </div>
</template>

<style lang="scss" scoped>
nav {
  position: sticky;
  z-index: 3;
  top: 0;
}

ul {
  list-style: none;
}

li {
  padding: 0 1rem;
  font-size: 15px;
  cursor: pointer;
}

span {
  padding: 0 0.8rem;
  cursor: pointer;
}

.navLateral {
  position: fixed;
  z-index: 5;
  top: 20%;
  right: 0;
}
</style>
