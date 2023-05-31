<script >

export default {
  components: {
    nome: "ButtonCustom",
  },
  props: {
    text:String,
  }
}
</script>


<template>
  <button class="btn px-3 fw-bold">{{ text }}</button>
</template>


<style lang="scss" scoped>

</style>
