<template>
  <v-container class=" blue lighten-4 py-5 my-0 ContentNoticia" fluid>
    <v-row no-gutters style="flex-wrap: nowrap" class="d-flex flex-column flex-md-row align-center align-md-left">
      <v-col cols="2" class=" flex-grow-0 d-flex justify-center  flex-shrink-0">

        <div class="d-flex justify-center flex-column px-10 py-auto">
          <v-icon x-large color="darken"> mdi-ninja </v-icon>
          <v-btn outlined class="my-3"> ver mas </v-btn>

          <div class=" my-0 d-flex flex-row ">
            <v-btn fab x-small class="mx-1" elevation="0" color="transparent">
              <v-icon medium color=" darken" class="px-2"> mdi-facebook</v-icon>
            </v-btn>

            <v-btn fab x-small class="mx-1" elevation="0" color="transparent">
              <v-icon medium color=" darken" class="px-2">
                mdi-instagram</v-icon
              >
            </v-btn>

            <v-btn fab x-small class="mx-1" elevation="0" color="transparent">
              <v-icon medium color=" darken" class="px-2"> mdi-youtube</v-icon>
            </v-btn>
          </div>
        </div>
      </v-col>

      <v-col
        cols="1"
        style="min-width: 100px; max-width: 100%"
        class="flex-grow-1 flex-shrink-0"      
      >
        <v-card class=" pa-md-2" elevation="0" color="transparent" >
          <v-tabs v-model="tab" class="pa-md-2  tabsNoticia" >
            <v-tabs-slider></v-tabs-slider>
            <v-tab
              v-for="item in items"
              :key="item.tab"
              class=" mx-5 mx-md-8"
              color="deep-purple accent-4"
            >
              {{ item.tab }}
            </v-tab>
          </v-tabs>

          <v-tabs-items v-model="tab" class="itemNoticia">
            <v-tab-item v-for="item in items" :key="item.tab" >
              <v-card flat >
                <v-card-text >
                  <v-sheet class="mx-auto" max-width="1200" >
                    <v-slide-group
                      v-model="model"
                      class=""
                      multiple
                      show-arrows     
                    >
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
                          <v-row
                          
                            class="fill-height"
                            align="center"
                            justify="center"
                          >
                            <v-scale-transition >
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
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      tab: null,
      items: [
        { tab: "Puerto Vallarta", content: "Puerto Vallarta" },
        { tab: "Nayarit", content: "Nayarit" },
       
      ],
      model: [],
    };
  },
};
</script>

<style>

.tabsNoticia.theme--light.v-tabs>.v-tabs-bar {
    background-color: transparent;
}
.container.indigo.lighten-4.py-10.ContentNoticia.container--fluid {
    background-color: #c5cae9!important;
}
.v-window.itemNoticia.v-item-group.theme--light.v-tabs-items {
    background-color: transparent;
}

.itemNoticia .v-card.v-card--flat.v-sheet.theme--light {
    background-color: transparent !important;
}
.itemNoticia .theme--light.v-sheet {
     background-color: transparent !important ; 

}
</style>