<template>
  <v-card class=""  elevation="0">
    <v-tabs v-model="tab" class="pa-md-5" >
      <v-tabs-slider ></v-tabs-slider>
      <v-tab v-for="item in items" :key="item.tab" class="mx-8"  color="deep-purple accent-4">
        {{ item.tab }}
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item v-for="item in items" :key="item.tab">
        <v-card flat>
          <v-card-text
            >
            <v-sheet class="mx-auto"  max-width="1200">
              <v-slide-group v-model="model" class="" multiple show-arrows>
                <v-slide-item
                  v-for="n in 15"
                  :key="n"
                  v-slot="{ active, toggle }"
                >
                  <v-card
                    :color="active ? 'primary' : 'grey lighten-1'"
                    class="ma-1"
                    height="130"
                    width="211"
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
          </v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs-items>
  </v-card>
</template>

<script>
export default {
  data() {
    return {
      tab: null,
      items: [
        { tab: "Puerto Vallarta", content: "Puerto Vallarta" },
        { tab: "Nayarit", content: "Nayarit" },
        { tab: "Manzanillo", content: "Manzanillo" },
      ],
      model: [],
    };
  },
};
</script>

<style>
</style>