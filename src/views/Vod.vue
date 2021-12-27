<template>
  <div class="border0"  >
    <Menu />
    <galeria-vod />
    <Footer />
    

  </div>
</template>

<script>
import Menu from '../components/Menu.vue'
import GaleriaVod from "../components/GaleriaVod.vue";
import Footer from '../components/Footer.vue';
export default {
  name: "VOD",

  components: {
    GaleriaVod,
    Footer,
    Menu
    
  },
};
</script>

<style>
</style>