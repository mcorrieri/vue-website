<template>
  <div>
    <v-row dense>
      <v-col sm="12" md="12" lg="6">
        <TitleContainer />
        <AboutContainer />
      </v-col>
      <v-col sm="12" md="12" lg="6">
        <v-card>
          <v-img src="IMG_5434.jpg" max-height="600" max-width="600"></v-img>
        </v-card>
      </v-col>
    </v-row>
    <ExperienceContainer />
    <ProjectContainer />
    <v-row dense justify="center" class="d-flex align-center my-4">
      <v-col sm="12" md="12" lg="6">
        <v-img
          class="justify-center pa-3 rounded"
          src="aqua.jpg"
          max-height="600"
          max-width="600"
        ></v-img>
      </v-col>
      <v-col sm="12" md="12" lg="6">
        <v-img
          class="justify-center pa-3 rounded"
          src="baby-angel.jpg"
          max-height="600"
          max-width="600"
        ></v-img>
      </v-col>
    </v-row>
    <ContactContainer />
  </div>
</template>

<script setup>
import ContactContainer from "./ContactContainer.vue";
import ExperienceContainer from "./ExperienceContainer.vue";
import TitleContainer from "./TitleContainer.vue";
</script>

<style></style>
