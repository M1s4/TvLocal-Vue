<template>
  <v-sheet class="mx-auto my-15" elevation="0" max-width="1200">
    <div class="font-weight-bold text-button mx-10">
      <v-icon x-medium color="black darken-2 " class="mx-3 my-4" left> mdi-video-vintage </v-icon>
      VIDEO BAJO DEMANDA (VOD)
    </div>
    <v-slide-group
      v-model="model"
      class="pa-3"
      active-class="success"
      show-arrows
    >
      <v-slide-item v-for="n in 15" :key="n" v-slot="{ active, toggle }">
        <v-card
          :color="active ? undefined : 'grey lighten-1'"
          class="ma-1"
          height="200"
          width="140"
          @click="toggle"
        >
          <v-row class="fill-height" align="center" justify="center">
            <v-scale-transition>
              <v-icon
                v-if="active"
                color="white"
                size="48"
                v-text="'mdi-close-circle-outline'"
                class=""
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
};
</script>

<style>
</style>