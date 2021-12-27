<template>
  <nav>
    <v-app-bar app elevate-on-scroll >
      <v-app-bar-nav-icon
        class="grey--text"
        @click="drawer = !drawer"
      ></v-app-bar-nav-icon>
      <v-toolbar-title class="text-md-uppercase text-subtitle-2 grey--text">
        <div class="d-flex align-center">
          <v-toolbar-title>
                      <v-icon color="black  " prominent left>mdi-television-box</v-icon>

            LOCAL</v-toolbar-title>
        </div>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn
        fab
        x-small
        text
        href="https://mega.nz/file/1IxCgKZD#uS0Ppvwx5kVXpShWM7t9fbxOlUNvlOqGmUbmmKlZAkY"
        target="_blank"
        class="mx-0"
      >
        <v-icon> mdi-facebook</v-icon>
      </v-btn>

      <v-btn
        fab
        x-small
        text
        href="https://mega.nz/file/1IxCgKZD#uS0Ppvwx5kVXpShWM7t9fbxOlUNvlOqGmUbmmKlZAkY"
        target="_blank"
        class="mx-0"
      >
        <v-icon> mdi-instagram</v-icon>
      </v-btn>
      <v-btn
        fab
        x-small
        text
        href="https://mega.nz/file/1IxCgKZD#uS0Ppvwx5kVXpShWM7t9fbxOlUNvlOqGmUbmmKlZAkY"
        target="_blank"
        class="mx-0"
      >
        <v-icon> mdi-youtube</v-icon>
      </v-btn>
      <v-btn
        fab
        x-small
        text
        href="https://mega.nz/file/1IxCgKZD#uS0Ppvwx5kVXpShWM7t9fbxOlUNvlOqGmUbmmKlZAkY"
        target="_blank"
        class="mx-0"
      >
        <v-icon> mdi-twitter</v-icon>
      </v-btn>
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" app temporary color="white">
      <div class="d-flex flex-column align-center mt-15">
        <v-btn class="black--text my-3" text to="/"> INICIO </v-btn>
        <v-btn class="black--text my-3" to="/envivo" text> EN VIVO </v-btn>
        <v-btn class="black--text my-3" to="/peliculas" text> PELICULA</v-btn>
        <v-btn class="black--text my-3" to="/horario" text> HORARIO </v-btn>
        <v-btn class="black--text my-3" to="/vod" text> VOD </v-btn>
        <v-btn class="black--text my-3" to="/nosotros" text> NOSOTROS </v-btn>
        <v-btn class="black--text my-3" to="/contacto" text> CONTACTO </v-btn>
      </div>

      <v-spacer></v-spacer>
      <div class="text-center mt-13">
        <v-btn
          class="mx-1"
          color="black"
          href="https://www.facebook.com/mis4el.gutierrez"
          target="_blank"
          text
          dark
          x-small
          fab
        >
          <v-icon>mdi-facebook</v-icon>
        </v-btn>

        <v-btn class="mx-1" color="black" text x-small fab>
          <v-icon>mdi-instagram</v-icon>
        </v-btn>

        <v-btn
          class="mx-1"
          color="black"
          href="https://github.com/M1s4"
          target="_blank"
          text
          x-small
          fab
        >
          <v-icon>mdi-youtube</v-icon>
        </v-btn>

        <v-btn
          class="mx-1"
          color="black"
          href="https://www.linkedin.com/in/misael-gutierrez-lopez-1281018a/"
          target="_blank"
          text
          x-small
          fab
        >
          <v-icon>mdi-twitter</v-icon>
        </v-btn>
      </div>
    </v-navigation-drawer>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      drawer: false,
    };
  },
};
</script>

<style>
</style>