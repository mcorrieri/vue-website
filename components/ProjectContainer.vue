<template>
  <v-card class="my-3">
    <v-card-title>Projects</v-card-title>
    <v-carousel
      cycle
      height="400"
      hide-delimiter-background
      show-arrows-on-hover
      class="my-3"
    >
      <template v-slot:prev="{ on, attrs }">
        <v-btn color="success" v-bind="attrs" v-on="on">Previous</v-btn>
      </template>
      <template v-slot:next="{ on, attrs }">
        <v-btn color="info" v-bind="attrs" v-on="on">Next</v-btn>
      </template>
      <v-carousel-item v-for="(slide, i) in slides" :key="i">
        <v-sheet :color="colors[i]" height="100%">
          <v-row class="fill-height" align="center" justify="center">
            <div class="text-h2">{{ slide }} Slide</div>
          </v-row>
        </v-sheet>
      </v-carousel-item>
    </v-carousel>
  </v-card>
</template>

<script>
export default {
  data() {
    return {
      colors: [
        "indigo",
        "warning",
        "pink darken-2",
        "red lighten-1",
        "deep-purple accent-4",
      ],
      slides: [
        "Fishy",
        "Covid-19 Vaccine Map",
        "Emoji Tic Tac Toe",
        "Big Apple Vacations",
        "Fifth",
      ],
    };
  },
};
</script>

<style scoped></style>
