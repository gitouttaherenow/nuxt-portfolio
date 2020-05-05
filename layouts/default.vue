<template>
  <div id="app">
    <Navbar />
    <h2>okay okay</h2>
    <router-view />
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar.vue";

export default {
  name: "app",
  components: {
    Navbar
  }
};
</script>

<style lang="stylus" scoped>
body
  background #000
</style>