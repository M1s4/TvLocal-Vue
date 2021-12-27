<template>
  <div>
    <Menu />
    <online />
    <slider-noticia />
    <slider-vod />
    <slider-pelicula />
    <Footer />
  </div>
</template>
  

<script>
import online from "../components/online.vue";
import SliderNoticia from "../components/SliderNoticia.vue";
import SliderVod from '../components/sliderVOD.vue'
import SliderPelicula from '../components/SliderPelicula.vue'
import Banner from '../components/Banner.vue'
import Footer from '../components/Footer.vue'
import Menu from '../components/Menu.vue'


export default {
  name: "En vivo",

  components: {
    online,
    SliderNoticia,
    SliderVod,
    SliderPelicula,
    Banner,
    Footer,
    Menu
  },
};
</script>

<style>
</style>