<template>
   <v-card elevation="0" class="mt-15">

    <v-toolbar elevation="0" >
      <v-toolbar-title class="font-weight-bold grey--text my-10 my-md-0 text-center"> 
        <v-icon left>
           mdi-calendar-multiselect
        </v-icon>
        HORARIO</v-toolbar-title>
    </v-toolbar>

      <v-tabs v-model="tabs" centered class="mt-13 mt-md-0" color="">
        <v-tab class="font-weight-black text-caption"> Puerto Vallarta </v-tab>
        <v-tab class="font-weight-black text-caption mx-6"> Nayarit </v-tab>
        <v-tab class="font-weight-black text-caption"> Manzanillo </v-tab>
      </v-tabs>

    <v-tabs-items v-model="tabs">
      <v-tab-item class="mt-md-15 contentTab">
        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>

        <v-divider class="mx-15"></v-divider>

        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>

        <v-divider class="mx-15"></v-divider>

        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>

        <v-divider class="mx-15"></v-divider>

        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>
        <v-divider class="mx-15"></v-divider>

        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>
        <v-divider class="mx-15"></v-divider>

        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>
        <v-divider class="mx-15"></v-divider>

        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>
      </v-tab-item>

      <v-tab-item class="mt-md-15 contentTab">
        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>

        <v-divider class="mx-15"></v-divider>

        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>

        <v-divider class="mx-15"></v-divider>

        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>

        <v-divider class="mx-15"></v-divider>

        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>

        <v-divider class="mx-15"></v-divider>

        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>

        <v-divider class="mx-15"></v-divider>

        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>

        <v-divider class="mx-15"></v-divider>

        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>
      </v-tab-item>

      <v-tab-item class="mt-md-15 contentTab">
        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>
        <v-divider class="mx-15"></v-divider>

        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>
        <v-divider class="mx-15"></v-divider>

        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>
        <v-divider class="mx-15"></v-divider>

        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>
        <v-divider class="mx-15"></v-divider>

        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>
        <v-divider class="mx-15"></v-divider>

        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>
        <v-divider class="mx-15"></v-divider>

        <v-card
          class="d-flex flex-column flex-md-row pa-6 my-6 my-md-0 mx-auto"
          max-width="900"
          elevation="0"
          color="grey lighten-3"
        >
          <div color="red" class="text-h5 font-weight-black">16:30</div>
          <div color="green" class="px-md-10">
            <v-card class="my-7 my-md-0">
              <v-img
                src="https://picsum.photos/350/165?random"
                max-height="300"
                class="grey darken-4"
              ></v-img>
            </v-card>
          </div>
          <div color="blue">
            <p class="text-button font-weight-bold my-0">TITULO DEL SITIO</p>
            <p class="text-body-2 font-weight-medium">
              Al contrario del pensamiento popular, el texto de Lorem Ipsum no
              es simplemente texto aleatorio. Tiene sus raices en una pieza
              clasica de la literatura del Latin.
            </p>
            <v-btn small outlined color="black"> ver capitulos </v-btn>
          </div>
        </v-card>
      </v-tab-item>
    </v-tabs-items>
  </v-card>
</template>

<script>
export default {
  data() {
    return {
      tabs: null,
      text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.",
    };
  },
};
</script>

<style>
.contentTab {
  background-color: #eeeeee;
}
</style>