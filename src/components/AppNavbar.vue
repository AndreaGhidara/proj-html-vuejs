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
            <div class="dropdown">
              <button class="btn dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
                {{ links }}
              </button>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Action</a></li>
                <li><a class="dropdown-item" href="#">Another action</a></li>
                <li><a class="dropdown-item" href="#">Something else here</a></li>
              </ul>
            </div>
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
@use '../variables.scss' as *;

button {
  border: none;

  &:focus {
    background-color: $Primary;
    color: #fff;
  }
}

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

// Social
.fa-facebook-f {

  &:hover {
    color: #3b5998;
  }
}

.fa-twitter {

  &:hover {
    color: #00ACEE;
  }
}

.fa-instagram {

  &:hover {
    color: orangered;
  }
}

.fa-linkedin-in {

  &:hover {
    color: #0e76a8;
  }
}

.navLateral {
  position: fixed;
  z-index: 5;
  top: 20%;
  right: 0;
}
</style>
