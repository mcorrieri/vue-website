<template>
  <v-card class="my-3">
    <v-card-title>Projects</v-card-title>
    <v-carousel
      v-if="$vuetify.breakpoint.mdAndUp"
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
            <div class="text-h2">
              <v-row dense align="center" justify="center">
                <v-col xs="6" sm="6" md="6" lg="6">
                  <v-card max-width="375">
                    <v-card-title>{{ slide.name }}</v-card-title>
                    <v-card-text class="text-center">
                      <v-icon large>{{ slide.iconA }}</v-icon>
                      <v-icon large>{{ slide.iconB }}</v-icon
                      ><v-icon large>{{ slide.iconC }}</v-icon
                      ><v-icon large>{{ slide.iconD }}</v-icon>
                      <v-icon large>{{ slide.iconE }}</v-icon>
                      <v-card-text>{{ slide.info }} </v-card-text>
                      <v-btn
                        outlined
                        v-if="slide.id !== 3"
                        :href="slide.demoLink"
                      >
                        <v-icon>{{ slide.youtubeIcon }}</v-icon>
                      </v-btn>
                      <v-btn outlined :href="slide.githubLink">
                        <v-icon class="mx-2">{{ slide.githubIcon }}</v-icon>
                      </v-btn>
                    </v-card-text>
                  </v-card>
                </v-col>
                <v-col sm="6" md="6" lg="6">
                  <v-img
                    contain
                    class="rounded"
                    :src="require(`@/assets/img/${slide.image}`)"
                    max-width="500"
                  />
                </v-col>
              </v-row>
            </div>
          </v-row>
        </v-sheet>
      </v-carousel-item>
    </v-carousel>
    <v-container v-else>
      <v-card>
        <v-row dense>
          <v-col v-for="slide in slides" :key="slide.id" :cols="slide.flex">
            <v-row dense align="center" justify="center">
              <v-col xs="6" sm="6" md="6" lg="6">
                <v-card max-width="375" outlined class="mb-2">
                  <v-card-title>{{ slide.name }}</v-card-title>
                  <v-card-text class="text-center">
                    <v-icon large>{{ slide.iconA }}</v-icon>
                    <v-icon large>{{ slide.iconB }}</v-icon
                    ><v-icon large>{{ slide.iconC }}</v-icon
                    ><v-icon large>{{ slide.iconD }}</v-icon>
                    <v-icon large>{{ slide.iconE }}</v-icon>
                    <v-card-text>{{ slide.info }} </v-card-text>
                    <v-img
                      contain
                      class="rounded mb-5"
                      :src="require(`@/assets/img/${slide.image}`)"
                      max-width="500"
                    />
                    <v-btn
                      outlined
                      v-if="slide.id !== 3"
                      :href="slide.demoLink"
                    >
                      <v-icon>{{ slide.youtubeIcon }}</v-icon>
                    </v-btn>
                    <v-btn outlined :href="slide.githubLink">
                      <v-icon class="mx-2">{{ slide.githubIcon }}</v-icon>
                    </v-btn>
                  </v-card-text>
                </v-card>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </v-card>
    </v-container>
  </v-card>
</template>

<script>
export default {
  data() {
    return {
      colors: ["indigo", "warning", "pink darken-2", "deep-purple accent-4"],
      slides: [
        {
          id: 1,
          name: "Fishy",
          image: "fishy.png",
          info: "Craigslist-based app that allows users to sell and buy fish while adding them to their virtual aquarium",
          iconA: "mdi-react",
          iconB: "mdi-language-javascript",
          iconC: "mdi-language-ruby-on-rails",
          iconD: "mdi-language-ruby",
          githubIcon: "mdi-github",
          githubLink: "https://github.com/mcorrieri/frontend-fishy",
          youtubeIcon: "mdi-youtube",
          demoLink: "https://youtu.be/iyt62efBkOM",
        },
        {
          id: 2,
          name: "Covid-19 Vaccine Map",
          image: "vaccine.png",
          info: "Public health app which graphically represents vaccination rates in the US using Chart.js",
          iconA: "mdi-react",
          iconB: "mdi-language-javascript",
          iconC: "mdi-language-ruby",
          githubIcon: "mdi-github",
          githubLink: "https://github.com/mcorrieri/Phase3-Frontend",
          youtubeIcon: "mdi-youtube",
          demoLink: "https://youtu.be/mXBkc_2mg1s",
        },
        {
          id: 3,
          name: "Emoji Tic Tac Toe",
          image: "emojipic.png",
          info: "Allows players to choose from a dropdown of emojis instead of using those antiquated Xs and Os",
          iconA: "mdi-react",
          iconB: "mdi-language-javascript",
          githubIcon: "mdi-github",
          githubLink: "https://github.com/mcorrieri/emoji-tic-tac-toe",
          youtubeIcon: null,
          demoLink: null,
        },
        {
          id: 4,
          name: "Big Apple Vacations",
          image: "vacation2.png",
          info: "Renters can book appointments using a calendar and can view or cancel any appointment on their appointments page",
          iconA: "mdi-react",
          iconB: "mdi-language-javascript",
          iconC: "mdi-language-ruby-on-rails",
          iconD: "mdi-language-ruby",
          githubIcon: "mdi-github",
          githubLink: "https://github.com/pjhg14/phase4-pair-project-frontend",
          youtubeIcon: "mdi-youtube",
          demoLink: "https://youtu.be/lTvMRwlDYf0",
        },
      ],
    };
  },
};
</script>

<style scoped></style>
