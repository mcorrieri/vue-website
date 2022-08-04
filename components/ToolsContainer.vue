<template>
  <v-card class="mt-3 pb-5">
    <v-card-title>Tools I Use</v-card-title>
    <v-card-text class="text-center">
      <v-tooltip top>
        <template v-slot:activator="{ on, attrs }">
          <v-icon
            v-on="on"
            v-bind="attrs"
            class="mx-2 mb-2"
            x-large
            color="green"
            >mdi-vuejs</v-icon
          >
        </template>
        <span>Vue</span>
      </v-tooltip>
      <v-tooltip top>
        <template v-slot:activator="{ on, attrs }">
          <v-icon
            v-on="on"
            v-bind="attrs"
            class="mx-2 mb-2"
            x-large
            color="blue"
            >mdi-vuetify</v-icon
          >
        </template>
        <span>Vuetify</span>
      </v-tooltip>
      <v-tooltip top>
        <template v-slot:activator="{ on, attrs }">
          <v-icon
            v-on="on"
            v-bind="attrs"
            class="mx-2 mb-2"
            x-large
            color="green"
            >mdi-nuxt</v-icon
          >
        </template>
        <span>Nuxt</span>
      </v-tooltip>
      <v-tooltip top>
        <template v-slot:activator="{ on, attrs }">
          <v-icon
            v-on="on"
            v-bind="attrs"
            class="mx-2 mb-2"
            x-large
            color="blue"
            >mdi-microsoft-azure-devops</v-icon
          >
        </template>
        <span>Azure DevOps</span>
      </v-tooltip>
      <v-tooltip top>
        <template v-slot:activator="{ on, attrs }">
          <v-icon
            v-on="on"
            v-bind="attrs"
            class="mx-2 mb-2"
            x-large
            color="yellow"
            >mdi-language-javascript</v-icon
          >
        </template>
        <span>JavaScript</span>
      </v-tooltip>
      <v-tooltip top>
        <template v-slot:activator="{ on, attrs }">
          <v-icon
            v-on="on"
            v-bind="attrs"
            class="mx-2 mb-2"
            x-large
            color="#90CAF9"
            >mdi-react</v-icon
          >
        </template>
        <span>React</span>
      </v-tooltip>
      <v-tooltip top>
        <template v-slot:activator="{ on, attrs }">
          <v-icon v-on="on" v-bind="attrs" class="mx-2 mb-2" x-large color="red"
            >mdi-language-ruby-on-rails</v-icon
          >
        </template>
        <span>Ruby on Rails</span>
      </v-tooltip>
      <v-tooltip top>
        <template v-slot:activator="{ on, attrs }">
          <v-icon v-on="on" v-bind="attrs" class="mx-2 mb-2" x-large color="red"
            >mdi-language-ruby</v-icon
          >
        </template>
        <span>Ruby</span>
      </v-tooltip>
      <v-tooltip top>
        <template v-slot:activator="{ on, attrs }">
          <v-icon v-on="on" v-bind="attrs" class="mx-2 mb-2" x-large
            >mdi-github</v-icon
          >
        </template>
        <span>GitHub</span>
      </v-tooltip>
      <v-tooltip top>
        <template v-slot:activator="{ on, attrs }">
          <v-icon
            v-on="on"
            v-bind="attrs"
            class="mx-2 mb-2"
            x-large
            color="#FDD835"
            >mdi-firebase</v-icon
          >
        </template>
        <span>Firebase</span>
      </v-tooltip>
      <v-tooltip top>
        <template v-slot:activator="{ on, attrs }">
          <v-icon
            v-on="on"
            v-bind="attrs"
            class="mx-2 mb-2"
            x-large
            color="blue"
            >mdi-material-ui</v-icon
          >
        </template>
        <span>MUI</span>
      </v-tooltip>
      <v-tooltip top>
        <template v-slot:activator="{ on, attrs }">
          <v-icon
            v-on="on"
            v-bind="attrs"
            class="mx-2 mb-2"
            x-large
            color="#EF6C00"
            >mdi-language-html5</v-icon
          >
        </template>
        <span>HTML</span>
      </v-tooltip>
    </v-card-text>
  </v-card>
</template>

<script setup></script>

<style scoped></style>
