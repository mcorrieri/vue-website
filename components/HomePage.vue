<template>
  <div>
    <v-card class="mb-3">
      <v-card-title>Michael Corrieri</v-card-title>
      <v-card-subtitle>Software Developer</v-card-subtitle>
      <v-spacer></v-spacer>
      <v-img src="IMG_5434.jpg" max-height="300" max-width="300"></v-img>
    </v-card>

    <AboutContainer />
    <ProjectContainer />
    <ContactContainer />
  </div>
</template>

<script setup>
import ContactContainer from "./ContactContainer.vue";
</script>

<style></style>
