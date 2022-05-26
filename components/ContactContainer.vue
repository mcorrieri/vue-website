<template>
  <v-card class="mt-3 pb-5">
    <v-card-title>Contact Me</v-card-title>
    <div class="text-center">
      <v-chip large class="mx-5" color="primary" text-color="white">
        <v-avatar left>
          <v-icon>mdi-account-circle</v-icon>
        </v-avatar>
        LinkedIn
      </v-chip>

      <v-chip large class="mx-5" color="red" text-color="white">
        <v-avatar left>
          <v-icon>mdi-email-fast-outline</v-icon>
        </v-avatar>
        Email
      </v-chip>

      <v-chip large class="mx-5" color="orange" text-color="white">
        <v-avatar left>
          <v-icon>mdi-github</v-icon>
        </v-avatar>
        GitHub
      </v-chip>
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
