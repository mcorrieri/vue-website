<template>
  <v-card class="mt-3 pb-5" outlined>
    <v-card-title>Contact Me</v-card-title>
    <div
      class="text-center"
      :class="{
        'text-h2': $vuetify.breakpoint.smAndDown,
        'text-center mb-2': $vuetify.breakpoint.mdAndUp,
      }"
    >
      <v-btn
        href="https://www.linkedin.com/in/michaelcorrieri/"
        large
        color="primary"
        text-color="white"
      >
        <v-avatar left>
          <v-icon>mdi-account-circle</v-icon>
        </v-avatar>
        LinkedIn
      </v-btn>

      <v-btn
        href="mailto:mlcorrieri@gmail.com"
        large
        color="red"
        text-color="white"
      >
        <v-avatar left>
          <v-icon>mdi-email-fast-outline</v-icon>
        </v-avatar>
        Email
      </v-btn>

      <v-btn
        href="https://github.com/mcorrieri"
        large
        color="orange"
        text-color="white"
      >
        <v-avatar left>
          <v-icon>mdi-github</v-icon>
        </v-avatar>
        GitHub
      </v-btn>
    </div>
  </v-card>
</template>

<script>
export default {
  methods: {
    close() {
      alert("Chip close clicked");
    },
  },
};
</script>

<style scoped></style>
