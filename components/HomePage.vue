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
    <ContactContainer />
  </div>
</template>

<script setup>
import ContactContainer from "./ContactContainer.vue";
import ExperienceContainer from "./ExperienceContainer.vue";
import TitleContainer from "./TitleContainer.vue";
</script>

<style></style>
