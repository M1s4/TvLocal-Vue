<template>
  <v-card class="px-4 px-md-15 mt-5 mt-md-15 mx-auto" fluid elevation="0">
    <p class="font-weight-black text-button text-md-h6 pb-2">
      <v-icon left color="black" > mdi-television-play </v-icon>
      SIGUE VIENDO TUS CAPITULOS
    </p>

    <v-card class="mt-3 mb-3 ml-auto" width="333" elevation="0">
      <v-select :items="Dias" label="Escoge el dia"></v-select>
    </v-card>

    <v-row class="fill-height" align="center" justify="center">
      <template v-for="(item, i) in items">
        <v-col :key="i" cols="6" md="2" class="pa-1">
          <v-hover v-slot="{ hover }">
            <v-card
              :elevation="hover ? 6 : 0"
              :class="{ 'on-hover': hover }"
              class="my-3 rounded-0"
              
            >
              <v-img
                :src="item.img"
                height="120"
                min-height="100"
                gradient="to top right, rgba(33,33,33,.33), rgba(33,33,33,.7)"
              >
                <v-card-title class="text-h6 white--text">
                  <v-row
                    class="fill-height flex-column mt-15"
                    justify="space-between"
                  >
                    <div class="">
                      <v-btn fab x-small color="#E0E0E0" absolute left>
                        <v-icon color="black" small> mdi-play </v-icon>
                      </v-btn>
                    </div>
                  </v-row>
                </v-card-title>
              </v-img>
              <div class="d-flex flex-row px-3 pt-3 pa-0 ">
                <p class="font-weight-black text-title pa-0 ma-0 grey--text text--darken-2" color="#9E9E9E">
                  EP1 - 5 JUL, 2020
                </p>
              </div>
              <p
                class="
                  text-subtitle-2
                  font-weight-black
                  text-left
                  px-3
                  pa-0
                  ma-0
                  pb-0 pb-3
                "
              >
                NOMBRE DE LA PELICULA
              </p>
            </v-card>
          </v-hover>
        </v-col>
      </template>
    </v-row>

  </v-card>

</template>

<script>
export default {
  data: () => ({
    icons: ["mdi-rewind", "mdi-play", "mdi-fast-forward"],
    items: [
      {
        title: "New Releases",
        text: `It's New Release Friday`,
        horario: "16:20",
        horario2: "20:16",
        subtext: "Newly released songs. Updated daily.",
        img: "https://images.unsplash.com/photo-1519241047957-be31d7379a5d?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=870&q=80",
      },
      {
        title: "Rock",
        text: "Greatest Rock Hits",
        subtext: "Lose yourself in rock tunes.",
        horario: "16:20",
        horario2: "20:16",
        img: "https://images.unsplash.com/photo-1620003118880-41b22176af1b?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=387&q=80",
      },
      {
        title: "Mellow Moods",
        text: "Ambient Bass",
        subtext: "Chill beats to mellow you out.",
        horario: "16:20",
        horario2: "20:16",
        img: "https://images.unsplash.com/photo-1620003117981-b8b8302fa71e?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=871&q=80",
      },
      {
        title: "Mellow Moods",
        text: "Ambient Bass",
        subtext: "Chill beats to mellow you out.",
        horario: "16:20",
        horario2: "20:16",
        img: "https://images.unsplash.com/photo-1595495529106-adb18dfe16a8?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=870&q=80",
      },
      {
        title: "Mellow Moods",
        text: "Ambient Bass",
        subtext: "Chill beats to mellow you out.",
        horario: "16:20",
        horario2: "20:16",
        img: "https://images.unsplash.com/photo-1593305841991-05c297ba4575?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=757&q=80",
      },
      {
        title: "Mellow Moods",
        text: "Ambient Bass",
        subtext: "Chill beats to mellow you out.",
        horario: "16:20",
        horario2: "20:16",
        img: "https://images.unsplash.com/photo-1596405367208-63505402f113?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=774&q=80",
      },
      {
        title: "Mellow Moods",
        text: "Ambient Bass",
        subtext: "Chill beats to mellow you out.",
        horario: "16:20",
        horario2: "20:16",
        img: "https://images.unsplash.com/photo-1596405367208-63505402f113?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=774&q=80",
      },
      {
        title: "Mellow Moods",
        text: "Ambient Bass",
        subtext: "Chill beats to mellow you out.",
        horario: "16:20",
        horario2: "20:16",
        img: "https://images.unsplash.com/photo-1534949378632-3e4e87ec219f?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=870&q=80",
      },
      {
        title: "Mellow Moods",
        text: "Ambient Bass",
        subtext: "Chill beats to mellow you out.",
        horario: "16:20",
        horario2: "20:16",
        img: "https://images.unsplash.com/photo-1557804506-e969d7b32a4b?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=845&q=80",
      },
      {
        title: "Mellow Moods",
        text: "Ambient Bass",
        subtext: "Chill beats to mellow you out.",
        horario: "16:20",
        horario2: "20:16",
        img: "https://images.unsplash.com/photo-1597575732103-9f6d068cfa9f?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=387&q=80",
      },
      {
        title: "Mellow Moods",
        text: "Ambient Bass",
        subtext: "Chill beats to mellow you out.",
        horario: "16:20",
        horario2: "20:16",
        img: "https://images.unsplash.com/photo-1605810230434-7631ac76ec81?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=870&q=80",
      },
      {
        title: "Mellow Moods",
        text: "Ambient Bass",
        subtext: "Chill beats to mellow you out.",
        horario: "16:20",
        horario2: "20:16",
        img: "https://images.unsplash.com/photo-1510511233900-1982d92bd835?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=870&q=80",
      },
    ],
    Dias: ["Lunes", "Marte", "Jueves", "Viernes", "Sabado", "Domingo"],

    transparent: "rgba(255, 255, 255, 0)",
  }),
};
</script>

<style>
</style>