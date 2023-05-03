<script>
import Header from "./components/Header.vue"

export default {
  name: "App",
  components: {
    Header
  }
}
</script>

<template>
  <Header />
</template>

<style lang="scss">
@use "./style/main.scss" as *;
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
}

</style>