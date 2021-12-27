<template>
<div>
  <Menu />    
  <videoprograma />
  <galeria-capitulo />
  <slider-pelis class="my-13" />
  <Footer />
</div>    

</template>

<script>
  import Menu from '../components/Menu.vue'
import Videoprograma from '../components/Videoprograma.vue'
import GaleriaCapitulo from '../components/GaleriaCapitulo.vue'
import SliderPelis from '../components/SliderPelicula.vue'
import Footer from '../components/Footer.vue'
import Banner from '../components/Banner.vue'


export default {
 components:{
     Menu,
     Videoprograma,
     GaleriaCapitulo,
     SliderPelis,
     Footer,
     Banner
 }
}
</script>

<style>

</style>