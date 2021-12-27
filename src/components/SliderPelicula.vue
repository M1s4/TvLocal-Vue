
<template>
  <v-sheet class="mx-auto my-10" elevation="0" :width="width">
    <v-row  class="my-3 d-flex flex-column flex-md-row">
      <v-btn text class="font-weight-bold text-button mx-10 ">
        <v-icon color="black" class=" my-4" left>
          mdi-movie-open-play
        </v-icon>

        Peliculas de la semana
      </v-btn>

      <v-spacer></v-spacer>

      <v-btn  elevation="0" class="mx-15 mx-md-0">
        ver mas
        <v-icon right> mdi-arrow-top-right-thick </v-icon>
      </v-btn>
    </v-row>

    <v-slide-group v-model="model" class="pa-4" center-active show-arrows>
      <v-slide-item v-for="n in 15" :key="n" v-slot="{ active, toggle }">
        <v-card
          :color="active ? 'primary' : 'grey lighten-1'"
          class="ma-1"
          height="200"
          width="150"
          @click="toggle"
        >
          <v-row class="fill-height" align="center" justify="center">
            <v-scale-transition>
              <v-icon
                v-if="active"
                color="white"
                size="48"
                v-text="'mdi-close-circle-outline'"
              ></v-icon>
            </v-scale-transition>
          </v-row>
        </v-card>
      </v-slide-item>
    </v-slide-group>
  </v-sheet>
</template>

<script>
export default {
  data: () => ({
    model: null,
  }),
  computed: {
    width() {
      switch (this.$vuetify.breakpoint.name) {
        case "xs":
          return 350;
        case "sm":
          return 400;
        case "md":
          return 500;
        case "lg":
          return 1200;
        case "xl":
          return 800;
      }
    },
  },
};
</script>

<style>
</style>