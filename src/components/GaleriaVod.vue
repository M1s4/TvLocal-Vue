<template>
  <v-container class="pa-md-10 text-center mt-10">
    <div class="d-flex align-content-center my-10 text-align-start">
      <v-icon x-medium color="black">mdi-television-classic </v-icon>
      <p class="mb-0 mx-2 font-weight-black">VIDEO BAJO DEMANDA</p>
    </div>
    <v-row class="fill-height" align="center" justify="center">
      <template v-for="(item, i) in items">
        <v-col :key="i" cols="6" md="2" class="pa-1">
          <v-hover v-slot="{ hover }">
            <v-card :elevation="hover ? 6 : 0" :class="{ 'on-hover': hover }">
              <v-img :src="item.img" height="190" min-height="100">
                <v-card-title class="text-h6 white--text">
                  <v-row
                    class="fill-height flex-column mt-15 pt-15"
                    justify="space-between"
                  >
                      <v-btn fab x-small color="white" to="/prueba/programaTest">
                        <v-icon color="black" small> mdi-play </v-icon>
                      </v-btn>
                  </v-row>
                </v-card-title>
              </v-img>
              <div class="d-flex flex-row px-3 pt-5 pb-3">
                <v-icon left color="black" x-small >
                  mdi-clock
                </v-icon>
                <p class=" font-weight-bold text-md-subtitle-2 pa-0 ma-0">
                  {{ item.horario }} - {{item.horario2}}
                </p>
              </div>
              <p
                class="text-subtitle-2 font-weight-black text-left px-3 pa-0 ma-0 pb-3"
              >
                {{ item.text }}
              </p>
              <p></p>
            </v-card>
          </v-hover>
        </v-col>
      </template>
    </v-row>
  </v-container>
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
      {
        title: "Mellow Moods",
        text: "Ambient Bass",
        subtext: "Chill beats to mellow you out.",
        horario: "16:20",
        horario2: "20:16",
        img: "https://images.unsplash.com/photo-1581092802858-671713398c0b?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=870&q=80",
      },
      {
        title: "Mellow Moods",
        text: "Ambient Bass",
        subtext: "Chill beats to mellow you out.",
        horario: "16:20",
        horario2: "20:16",
        img: "https://images.unsplash.com/photo-1543449255-43e665de7553?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=870&q=80",
      },
      {
        title: "Mellow Moods",
        text: "Ambient Bass",
        subtext: "Chill beats to mellow you out.",
        horario: "16:20",
        horario2: "20:16",
        img: "https://images.unsplash.com/photo-1608737739007-f0019bc67f59?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=376&q=80",
      },
      {
        title: "Mellow Moods",
        text: "Ambient Bass",
        subtext: "Chill beats to mellow you out.",
        horario: "16:20",
        horario2: "20:16",
        img: "https://images.unsplash.com/photo-1581092795360-fd1ca04f0952?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=387&q=80",
      },
      {
        title: "Mellow Moods",
        text: "Ambient Bass",
        subtext: "Chill beats to mellow you out.",
        horario: "16:20",
        horario2: "20:16",
        img: "https://images.unsplash.com/photo-1594434885674-0a15708152bf?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=387&q=80",
      },
      {
        title: "Mellow Moods",
        text: "Ambient Bass",
        subtext: "Chill beats to mellow you out.",
        horario: "16:20",
        horario2: "20:16",
        img: "https://images.unsplash.com/photo-1618193139062-2c5bf4f935b7?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=387&q=80",
      },
    ],
    transparent: "rgba(255, 255, 255, 0)",
  }),
};
</script>

<style scoped>
.v-card {
  transition: opacity 0.4s ease-in-out;
}

.v-card:not(.on-hover) {
  opacity: 0.6;
}

.show-btns {
  color: rgba(255, 255, 255, 1) !important;
}
</style>