<script>
import HeaderComp from "./components/HeaderComp.vue"
import MainComp from "./components/MainComp.vue"
import FooterComp from "./components/FooterComp.vue"

export default {
  name: "App",
  components: {
    HeaderComp,
    MainComp,
    FooterComp
  }
}
</script>

<template>
  <HeaderComp />
  <MainComp />
  <FooterComp />
</template>

<style lang="scss">
@use "./style/main.scss" as *;
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro:ital,wght@0,200;0,300;0,400;0,600;0,700;0,900;1,200;1,300;1,400;1,600;1,700;1,900&display=swap');

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  text-decoration: none;
  list-style: none;
  list-style-type: none;
}

body {
  font-family: 'Source Sans Pro', sans-serif;
  background: #fff;
  color: #1C1C1C;
  user-select: none;
}

</style>