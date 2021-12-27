<template>
  <v-container class="deep-orange lighten-4" fluid color="#FF80AB">
    <v-row no-gutters style="d-flex flex-wrap: nowrap;" class="d-flex flex-column flex-md-row align-center">
      <v-col cols="4" class="d-flex justify-center flex-grow-0 flex-shrink-0">
        <v-card 
        class="pa-2 d-flex flex-column align-center " 
        outlined 
        tile 
        color="transparent"
        
        >
          <div
            class="
              text-center
              font-weight-black
              text-h5
              font-roboto
              weight-600
              my-3
              red-lighten-5--text
            "
          >
            ¡ESCUCHANOS EN VIVO!
          </div>
          <div class="d-flex justify-center my-8">
            <v-btn-toggle
              v-model="toggle_exclusive"
              mandatory
              class="background:transparent !transparent;"
            >
              <v-btn outlined color="deep-orange accent-3">
                <div class="">
                  <div class="d-flex text-estaton">
                    <p class="font-weight-black mb-0">888.8</p>
                    <p class="font-weight-black mb-0">FM</p>
                  </div>
                  <p class="font-weight-regular mb-0 overline text-region">
                    PTO. VALLARTA
                  </p>
                </div>
              </v-btn>

              <v-btn class="mx-1" outlined color="deep-orange accent-3">
                <div>
                  <div class="d-flex text-estaton">
                    <p class="font-weight-black mb-0">888.8</p>
                    <p class="font-weight-black mb-0">FM</p>
                  </div>
                  <p class="font-weight-regular mb-0 overline text-region">
                    PTO. VALLARTA
                  </p>
                </div>
              </v-btn>

              <v-btn outlined color="deep-orange accent-3">
                <div class="">
                  <div class="d-flex text-estaton">
                    <p class="font-weight-black mb-0">888.8</p>
                    <p class="font-weight-black mb-0">FM</p>
                  </div>
                  <p class="font-weight-regular mb-0 overline text-region">
                    PTO. VALLARTA
                  </p>
                </div>
              </v-btn>
            </v-btn-toggle>
          </div>
        </v-card>
      </v-col>

      <v-col
        cols="4"
        style="min-width: 100px; max-width: 100%"
        class="flex-grow-1 flex-shrink-0"
      >
        <v-card class="pa-2" outlined tile color="transparent">
          <div>
            <div
              class="
                text-center
                font-weight-black
                text-h6
                font-roboto
                weight-600
                my-3
                grey--text
                text--lighten-5
              "
            >
              ESTAS ESCUCHANDO 88.8 FM
            </div>
            <div class="d-flex justify-center my-8">
              <audio controls color="transparent">
                <source
                  src="https://www.free-stock-music.com/music/mixaund-sunrise.mp3"
                  codecs="mp3"
                />

                Your browser does not support the audio element.
              </audio>
            </div>
          </div>
        </v-card>
      </v-col>

      <v-col
        cols="4"
        style="min-width: 100px"
        class="flex-grow-0 flex-shrink-1"
      >
        <v-card class="pa-2 d-flex align-end flex-column justify-space-between" outlined tile color="transparent" height="100%">
         
            <v-icon large color="black darken-2 x-large" > mdi-radio-fm </v-icon>
            <p 
            class="font-weight-medium text-caption mb-0 black--text parrafoText" 
            >
              Es un hecho establecido hace demasiado
            </p>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      toggle_exclusive: undefined,
    };
  },
};
</script>

<style>
.v-application .overline {
  line-height: 1rem !important;
  font-size: 0.5rem !important;
}
p.font-weight-regular.mb-0.overline.text-region {
  font-size: 0.55rem !important;
}
.d-flex.text-estaton {
  font-size: 0.75rem !important;
}
.theme--light.v-btn-toggle:not(.v-btn-toggle--group) {
  background: transparent !important;
}
.parrafoText {
    width: 165px;
    text-align: right;
}
</style>  