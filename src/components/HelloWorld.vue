<template>
  <v-carousel hide-delimiters vertical show-arrows-on-hover :height="height" >
    <v-carousel-item
      v-for="(item, i) in items"
      :key="i"
      :src="item.src"
      class="mt-15"
      gradient="to top right, rgba(33,33,33,.22), rgba(33,33,33,.7)"

    >
      <v-spacer> </v-spacer>
      <v-card class="mt-md-15 d-flex flex-column flex-md-row align-center align-md-start" height="350" elevation="0" color="transparent" app>
        
        <v-card class="pl-15 pt-10" width="430" color="transparent" elevation="0">
          <p class="font-weight-black white--text text-h3">TITULO DEL CAPITULO</p>
          <p class=" pr-10 text--lighten white--text py-3"> Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s</p>
          <p class="white--text text-caption font-weight-bold ma-1">
            lun - 10:00 - 11:00 am
          </p>
          <v-btn tile class="white--text mx-auto" color="#0092F3" elevation="0" to="/prueba/programaTest"> ver capitulos </v-btn>
        </v-card>
         <v-spacer></v-spacer>
        <v-card class="d-flex flex-md-column  pr-15 mt-6 mt-md-15" color="transparent" elevation="0">
          <v-btn class="my-2" text fab>
          <v-icon  color="white" small> mdi-facebook </v-icon>

          </v-btn>
          <v-btn class="my-2" text fab>
                      <v-icon  color="white" small> mdi-whatsapp </v-icon>

          </v-btn>
          <v-btn class="my-2" text fab>
          <v-icon  color="white" small> mdi-instagram </v-icon>

          </v-btn>
        </v-card>

      </v-card>
    </v-carousel-item>
  </v-carousel>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg",
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/sky.jpg",
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/bird.jpg",
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/planet.jpg",
        },
      ],
    };
  },
  computed: {
    height() {
      switch (this.$vuetify.breakpoint.name) {
        case "xs":
          return 600;
        case "sm":
          return 500;
        case "md":
          return 500;
        case "lg":
          return 600;
        case "xl":
          return 800;
      }
    },
  },
};
</script>

