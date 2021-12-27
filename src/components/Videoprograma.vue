<template>
  <v-card fluid class="px-0 my-0 py-0" elevation="0">
    <iframe
      class="px-0 pa-0 ma-0"
      width="100%"
      height="550px"
      src="https://www.youtube.com/embed/vpaPWuDQUcc"
      title="YouTube video player"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen
    >
    </iframe>
    <v-card class="py-6 px-4 px-md-15 mx-auto"  elevation="0">
      <p class="font-weight-black text-h6">TITULO DEL PROGRAMA</p>
      <div class="d-flex flex-column flex-md-row flex-md-row pt-1">
        <div class="d-flex flex-row  px-0">
          <v-btn text>
            <v-icon left> mdi-calendar</v-icon>
            Lunes
          </v-btn>
          <v-btn text>
            <v-icon left>mdi-clock</v-icon>
            22:00 Horas
          </v-btn>
        </div>
        <v-spacer></v-spacer>
        <div class="d-flex justify-center align-center py-2 py-md-0">
          <p class="text-body-2 text-md-body-2 font-weight-medium px-5 pl-0 mb-0">
            comparte en redes:
          </p>
          <div class="d-flex flex-md-row">
            <v-btn fab text small class="mx-1">
              <v-icon small> mdi-facebook</v-icon>
            </v-btn>
            <v-btn fab text small class="mx-1">
              <v-icon small>mdi-instagram</v-icon>
            </v-btn>
            <v-btn fab text small class="mx-1">
              <v-icon small>mdi-whatsapp</v-icon>
            </v-btn>
          </div>
        </div>
      </div>
      <p class="font-weight-medium pt-3 pt-md-6">
        Llega siempre un tiempo en que hay que elegir entre la contemplación y
        la acción. Eso se llama hacerse un hombre. Esos desgarramientos son
        espantosos, pero para un corazón orgulloso no puede haber término medio.
        Existe Dios o el tiempo, esta cruz o esta espada. Este mundo tiene un
        sentido más alto que supera a sus agitaciones o nada es cierto sino esas
        agitaciones. Hay que vivir con el tiempo y morir con él o sustraerse a
        él para una vida más grande. Sé que se puede transigir y que se puede
        vivir en el siglo y creer en lo eterno. Eso se llama aceptar. Pero me
        opongo a este término y quiero todo o nada. Si elijo la acción, no se
        crea que la contemplación es para mí una tierra desconocida. Pero no
        puede dármelo todo y, privado de lo eterno, quiero aliarme con el
        tiempo. No quiero tener en cuenta la nostalgia ni la amargura y lo único
        que quiero es ver con claridad.
      </p>
    </v-card>
  </v-card>
</template>

<script>
export default {};
</script>

<style>
</style>