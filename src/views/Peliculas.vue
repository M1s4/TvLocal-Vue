<template >
  <div class="border0">
    <Menu />
    <galeria />
    <Footer />
  </div>
</template>

<script>
import Galeria from "../components/galeria.vue";
import Footer from "../components/Footer.vue";
import Banner from "../components/Banner.vue";
  import Menu from '../components/Menu.vue'

export default {
  name: "Peliculas",

  components: {
    Galeria,
    Footer,
    Banner,
          Menu

  },
};
</script>

<style>
</style>