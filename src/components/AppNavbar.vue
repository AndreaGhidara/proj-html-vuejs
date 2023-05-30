<script >

export default {
  components:{
    nome:"AppNavbar"
  }
}
</script>

<template>
  <nav class="container d-flex justify-content-between align-items-center py-3 px-0">
        <div>
          <img style="width: 10rem;" src="/dark-logo.png" alt="">
        </div>
        <div>
          <ul class="d-flex m-0">
            <li>Home <i class="fa-solid fa-angle-down"></i></li>
            <li>Pages <i class="fa-solid fa-angle-down"></i></li>
            <li>Courses <i class="fa-solid fa-angle-down"></i></li>
            <li>Features <i class="fa-solid fa-angle-down"></i></li>
            <li>Blog <i class="fa-solid fa-angle-down"></i></li>
            <li>Shop <i class="fa-solid fa-angle-down"></i></li>
          </ul>
        </div>
        <div>
          <span><i class="fa-brands fa-facebook-f"></i></span>
          <span><i class="fa-brands fa-twitter"></i></span>
          <span><i class="fa-brands fa-instagram"></i></span>
          <span><i class="fa-brands fa-linkedin-in"></i></span>
        </div>
  </nav>
</template>

<style lang="scss" scoped>
$White:#ffffff;

  nav{
    background-color: $White;
  }

  ul{
    list-style: none;
  }

  li{
    padding: 0 1rem;
    font-size: 15px;
  }

  span{
    padding: 0 0.8rem;
  }
</style>
