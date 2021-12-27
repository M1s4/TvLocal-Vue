<template>
<div class="border0">
  <Menu />
  <hello-world />
  <programacion-slider />
  <slider-pelicula />
  <slider-noticia /> 
  <Reproductor class="my-10 my-md-15"/>
  <slider-vod />
  <Footer/>
</div>

</template>


<script>
  import HelloWorld from '../components/HelloWorld'
  import ProgramacionSlider from '../components/sliderProgramacion.vue'
  import Banner from '../components/Banner.vue'
  import SliderPelicula from '../components/SliderPelicula.vue'
  import SliderNoticia from '../components/SliderNoticia.vue'
  import Reproductor from '../components/Reproductor.vue'
  import SliderVod from '../components/sliderVOD.vue'
  import Footer from '../components/Footer.vue'
  import Menu from '../components/Menu.vue'


  export default {
    name: 'Home',

    components: {
      HelloWorld,
      ProgramacionSlider,
      Banner,
      SliderPelicula,
      SliderNoticia,
      Reproductor,
      SliderVod,
      Footer,
      Menu
    },
  }
</script>
