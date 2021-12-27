<template>
  <v-item-group class="mb-10">
    <v-container>
      <div>
      <div class="font-weight-black mt-15 py-5 pt-md-10 text-button">
        <v-icon color="black" class="mx-3 my-4" left> mdi-movie-open-play </v-icon>
        PELICULAS DE LA SEMANA
      </div>
      <div class="d-flex align-center  pb-4 justify-end">
        <p class="font-weight-black text-caption ma-0 pa-0">COMPARTE EN TUS REDES :</p>
        <div>
          <v-btn text fab x-small>
            <v-icon>mdi-facebook</v-icon>
          </v-btn>
          <v-btn text fab x-small>
            <v-icon>mdi-instagram</v-icon>
          </v-btn>
          <v-btn text fab x-small>
            <v-icon>mdi-whatsapp</v-icon>
          </v-btn>
        </div>
      </div>
      </div>


      <v-row class="mx-2">
        <v-col v-for="n in 18" :key="n" cols="6" md="2" class=" pa-1">
          <v-item v-slot="{ active, toggle }">
            <v-card
              :color="active ? 'cyan lighten-4' : 'transparent'"
              class="d-flex flex-column align-left outlined-0"
              elevation="0"              
              height="auto"
              @click="toggle"
              @click.stop="dialog = true"
            >
              
              <v-img
                :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
                :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}`"
                aspect-ratio="1"
                class="grey lighten-2"
                height="200"
                width="100%"
              >
              
                <template v-slot:placeholder>
                  <v-row
                    class="fill-height ma-0"
                    align="center"
                  >
                    <v-progress-circular
                      indeterminate
                      color="grey lighten-5"
                    ></v-progress-circular>
                  </v-row>
                </template>
              </v-img>
              <v-card-subtitle class="font-weight-black mx-0 px-0 mt-0 pt-3 pb-1"> 1,000 miles of wonder </v-card-subtitle>
            </v-card>
          </v-item>
        </v-col>
      </v-row>
    </v-container>

    <v-dialog v-model="dialog" max-width="785" height="500" fluid>
      <v-card>
        <video autoplay="" loop="" controls="" width="auto" height="480">
          <source
            type="video/mp4"
            src="https://endtest-videos.s3-us-west-2.amazonaws.com/documentation/endtest_data_driven_testing_csv.mp4"
          />
        </video>
        <v-card-title class="font-weight-black text-button">
          TITULO DE LA PELICULA -
          <p class="font-weight-bold text-heading6 my-0">Nombre Autor</p>
        </v-card-title>
        <div class="font-weight-medium text-caption my-3 mx-8" color="grey">
          2017 - 108min
        </div>

        <v-card-text class="font-weight-black">
          Lorem Ipsum is simply dummy text of the printing and typesetting
          industry. Lorem Ipsum has been the industry's standard dummy text ever
          since the 1500s, when an unknown printer took a galley of type and
          scrambled it to make a type specimen book.
        </v-card-text>

        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn
            class="text-align-end"
            color="black darken-1"
            text
            @click="dialog = false"
            z-index="2"
          >
            Cerrar
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </v-item-group>
</template>

<script>
export default {
  data() {
    return {
      dialog: false,
    };
  },
};
</script>

<style>
</style>