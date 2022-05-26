<template>
  <div>
    <v-row dense>
      <v-col sm="12" md="12" lg="6">
        <TitleContainer />
      </v-col>
      <v-col sm="12" md="12" lg="6">
        <AboutContainer />
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
