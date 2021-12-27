<template>
  <div class="mt-15 contentPrincipal" elevation="2">
    <v-card
      class="mx-auto "
      elevation="0"
      height="510"
      max-width="100%"
      color="secondary"
      absolute="absolute"
    >
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3734.3382529530127!2d-105.23406968557079!3d20.615065007149067!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x8421454528047edb%3A0x7de0f44b3e82f8ec!2sParque%20Miguel%20Hidalgo!5e0!3m2!1ses!2smx!4v1634077255854!5m2!1ses!2smx"
        width="100%"
        class="mt-n16 mt-md-0"
        height="100%"
        style="border: 0"
        allowfullscreen=""
        loading="lazy"
      ></iframe>
        <v-btn color="cyan darken-3" dark absolute  top right fab >
        <v-icon>mdi-eye-remove</v-icon>
      </v-btn>


    </v-card>

    <v-card
      :class="['ml-md-15', 'cardForm', 'px-8', displays]"
      height="550"
      max-width="600"
      color="#1B2237"
    >
    
      <div class="text-h6 font-weight-bold white--text text-center pt-5">
        ¿QUIERES ANUNCIARTE?
      </div>
      <form color="grey" class="mt-3">
        <v-text-field
          :counter="10"
          label="Nombre"
          required
        ></v-text-field>
        <v-text-field
          label="Correo"
          required
        ></v-text-field>
        <v-text-field
          :counter="7"
          label="Telefono"
          required
        ></v-text-field>
        <v-textarea
          clearable
          clear-icon="mdi-close-circle"
          label="Text"
          color="white"
          class="white--text"
        ></v-textarea>

        <v-btn
          class="mt-2 py-6 white--text"
          block
          rounded
          color="#3082B9"
        >
          ENVIAR
          <v-icon right> mdi-send-circle </v-icon>
        </v-btn>
        <v-btn
          class="my-3 py-6"
          color="cyan"
          dark
          rounded
          block
        >
          LIMPIAR
          <v-icon right>mdi-broom</v-icon>
        </v-btn>
      </form>
    </v-card>
  </div>
</template>

<script>
export default {
  data: () => ({
    direction: "top",
    fab: false,
    fling: false,
    hover: false,
    tabs: null,
    top: false,
    right: true,
    bottom: true,
    left: false,
    transition: "slide-y-reverse-transition",
    displays: 'd-block',
  }),

};
</script>

<style>
.cardForm {
  z-index: 3;
  margin-top: -530px;
}
.mt-15.contentPrincipal {
  margin-top: 160px !important;
}
.theme--light.v-label {
  color: white;
}
input {
  border-bottom: 1px solid grey;
  color: burlywood;
}
.theme--light.v-input textarea {
  border-bottom: 1px solid grey;
  height: 90px;
  color: white;
}
.theme--light.v-counter {
  color: grey;
}
</style>