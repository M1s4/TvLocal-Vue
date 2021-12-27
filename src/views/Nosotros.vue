<template>
  <div>
    <Menu />

    <content-nosotros />

    <Footer></Footer>
  </div>
</template>

<script>
import Menu from "../components/Menu.vue";
import ContentNosotros from "../components/ContentForm.vue";
import Footer from "../components/Footer.vue";
export default {
  name: "Nosotros",

  components: {
    Footer,
    Menu,
    ContentNosotros,
  },
};
</script>

<style>
.imgHistoria {
  height: 600px !important;
  margin-top: -35px;
  position: absolute;
}
.container.grey.lighten-5.px-0.contentHistoria.container--fluid.height {
  background-color: #e0e0e0 !important;
  height: 350px;
}
.tituloFlotante {
  margin-left: -35px;
}
.zIndex3 {
  z-index: 1;
}

.FirstContent {
  margin-top: -300px !important;
  position: relative !important;
  z-index: 3 !important;
  background-color: white !important;
  border-radius: 55px 55px 0px 0px !important;
}
</style>