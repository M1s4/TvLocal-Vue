<template>
   <div class="border0">
       <Menu />
       <slider-horario />
       <Footer />
   </div>
</template>

<script>
import Menu from '../components/Menu.vue'
import SliderHorario from '../components/SliderHorario.vue'
import Footer from '../components/Footer.vue'

export default {
  name: "Horario",

  components:{
    SliderHorario,
    Footer,
    Menu
  },

}
</script>

<style>

</style>