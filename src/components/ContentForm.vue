<template>
  <v-container class="pa-0" fluid>
    <v-container
      class="pa-0 d-flex flex-column flex-md-row justify-center mt-md-15"
      elevation="0"
      fluid
    >
      <v-col
        cols="12"
        class="
          d-flex
          flex-column
          justify-center
          text-right
          mt-md-15
          pr-5
          FirstContent          
        "
        elevation="0"
        sm="6"
        order="2"
        order-md="1"
      >
        <div
          class="
            d-flex
            flex-md-column
            font-weight-black
            text-left text-md-right text-h5 text-md-h3
            my-3
            mx-10
          ">
          <p class="pa-0 ma-0 pr-2">SOBRE</p>
          <p class="pa-0 ma-0">NOSOTROS</p>
        </div>

        <div class="pa-0 mt-n5">
          <v-btn class="my-md-10" elevation="0">
            <v-icon color="black" medium> mdi-arrow-top-right </v-icon>
          </v-btn>
        </div>

        <v-card
          max-width="580"
          elevation="0"
          class="
            text-body
            font-weight-text
            ml-auto
            text-center text-md-right
            mx-auto
            px-2
            my-6
          "
        >
          Lorem Ipsum is simply dummy text of the printing and 
          typesetting industry. Lorem Ipsum has been the industry's
           standard dummy text ever since the 1500s, when an unknown
            printer took a galley of type and scrambled it to make a
             type specimen book. It has survived not only five centuries,
        </v-card>
        <div>
          <v-btn elevation="0" class="my-3 my-md-10" depressed>
            CONTACTANOS
          </v-btn>
        </div>
        <v-btn
          ref="button"
          elevation="0"
          class="mx-auto"
          fab
          @click="$vuetify.goTo('#HistoyCont', linear)"
        >
          <v-icon x-large> mdi-chevron-down </v-icon>
        </v-btn>
      </v-col>

      <v-col cols="12" sm="6" class="mx-0 pa-0" order="1" order-md="2">
        <v-img
          lazy-src="https://picsum.photos/id/11/10/6"
          height="600px"
          max-width="100%"
          src="https://images.unsplash.com/photo-1486693128850-a77436e7ba3c?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80"
          aspect-ratio="2"
        ></v-img>
      </v-col>
    </v-container>

    <v-container
      class="grey lighten-4 px-0 contentHistoria my-md-15"
      fluid
      height="300px"
    >
      <v-row no-gutters justify="end">
        <v-col cols="12" sm="6" md="4" class="d-none d-md-block">
          <v-card class="" elevation="0" tile>
            <v-img
              lazy-src="https://picsum.photos/id/11/10/6"
              max-height="385"
              max-width="100%"
              src="https://picsum.photos/id/11/500/300"
              class="imgHistoria rounded-sm"
            ></v-img>
          </v-card>
        </v-col>

        <v-col cols="12" md="6" id="HistoyCont">
          <v-card class="mt-9 mt-md-5"  color="transparent" outlined tile>
            <v-btn
              elevation="8"
              class="ml-md-n16 white--text pl-15 py-7 pr-10 text-h6"
              color="black"
              >HISTORIA
            </v-btn>
            <div
              class="
                mt-8
                ml-md-0
                text-break
                font-weight-light
                rounded-lg
                px-7 px-md-10
                text-center text-md-left
              "
            >
              <p>
                Lorem Ipsum is simply dummy text of the printing and typesetting
                industry. Lorem Ipsum has been the industry's standard dummy
                text ever since the 1500s, when an unknown printer took a galley
                of type and scrambled it to make a type specimen book. It has
                survived not only five centuries, but also the leap into
                electronic typesetting, remaining essentially unchanged. It was
                popularised in the 1960s with the release of Letraset sheets
                containing Lorem Ipsum passages, and more recently with desktop
                publishing software like Aldus PageMaker including versions of
                Lorem Ipsum.
              </p>
            </div>
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <v-container class="pa-0 contentHistoria my-md-15" fluid height="300px">
      <v-row no-gutters justify="end" class="my-0">
        <v-col cols="12" sm="6" md="5" class="my-md-5 grey lighten-4 py-10">
          <v-card elevation="0" color="transparent" class="d-flex justify-end">
            <v-btn
              elevation="4"
              color="black"
              class="
                zIndex3
                white--text
                text-h6
                font-weight-black
                pl-13
                py-6
                pr-8
                ml-auto
                mr-md-n9
              "
              absolute
            >
              MISION
            </v-btn>
            <div
              class="
                font-weight-light
                mt-10 mt-md-10
                mx-10 mx-md-15
                text-center text-md-right
                pt-10
              "
            >
              Lorem Ipsum is simply dummy text of the printing and typesetting
              industry. Lorem Ipsum has been the industry's standard dummy text
              ever since the 1500s, It has survived not only five centuries, but
              also the leap into electronic typesetting,
            </div>
          </v-card>
        </v-col>
        <v-col cols="6" md="5" class="d-none d-md-block">
          <v-card elevation="0" color="yellow">
            <v-img
              height="300"
              src="https://images.unsplash.com/photo-1562673005-7693bd6d6e54?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=578&q=80"
            ></v-img>
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <v-container class="pa-0 contentHistoria my-md-15" fluid height="300px">
      <v-row no-gutters justify="start" class="my-0">
        <v-col cols="6" md="5" class="d-none d-md-block">
          <v-card elevation="0" color="yellow">
            <v-img
              height="300"
              src="https://images.unsplash.com/photo-1427348693976-99e4aca06bb9?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=870&q=80"
            ></v-img>
          </v-card>
        </v-col>

        <v-col cols="12" sm="6" md="5" class="my-md-5 grey lighten-4">
          <v-card elevation="0" color="transparent" class="d-flex">
            <v-btn
              elevation="4"
              color="black"
              class="
                zIndex3
                white--text
                text-h6
                font-weight-black
                pl-13
                py-6
                pr-8
                ml-auto ml-md-n9
                mt-6
              "
              absolute
            >
              VISION
            </v-btn>
            <div
              class="
                font-weight-light
                mt-10 mt-md-15
                mx-15
                text-left
                pt-md-10 pt-13
                pb-10
              "
            >
              Lorem Ipsum is simply dummy text of the printing and typesetting
              industry. Lorem Ipsum has been the industry's standard dummy text
              ever since the 1500s, It has survived not only five centuries, but
              also the leap into electronic typesetting,
            </div>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-container>
</template>

<script>
export default {};
</script>

<style>
</style>