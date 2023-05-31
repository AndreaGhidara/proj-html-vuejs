<script >

export default {
  nome:"AppNavbar",
  components:{
  
  },
  data(){
    return {
      navLink:["Home","Pages","Courses","Features","Blog","Shop",],
    }
  },
  methods: {

  },
  mounted(){

  }
}
</script>

<template>
  <nav class="container d-flex justify-content-between align-items-center py-4 px-0">
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
  </nav>
</template>

<style lang="scss" scoped>
  ul{
    list-style: none;
  }

  li{
    padding: 0 1rem;
    font-size: 15px;
    cursor: pointer;
  }

  span{
    padding: 0 0.8rem;
    cursor: pointer;
  }
</style>
