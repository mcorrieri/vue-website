<template>
  <div>
    <v-row>
      <v-col xs="12" sm="12" md="12" lg="12">
        <v-card>
          <v-card-title
            :class="{
              'text-h1': $vuetify.breakpoint.smAndDown,
              'text-h2 mb-2': $vuetify.breakpoint.mdAndUp,
            }"
            >Michael Corrieri</v-card-title
          >
          <v-card-subtitle class="text-h5">Software Developer</v-card-subtitle>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script setup></script>
