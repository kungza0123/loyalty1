<template>
    <v-container>
      <v-card class="mx-auto" max-width="500">
        <v-card-title class="text-center">
          Forgot Password
        </v-card-title>
        <v-card-text>
          <v-form @submit.prevent="submit">
            <v-text-field v-model="email" label="Email"></v-text-field>
            <v-btn type="submit" color="primary" class="mr-4">Submit</v-btn>
            <v-btn href="/" color="secondary">Cancel</v-btn>
          </v-form>
        </v-card-text>
      </v-card>
    </v-container>
  </template>
  
  <script>
  export default {
    data() {
      return {
        email: '',
      };
    },
    methods: {
      submit() {
        // Handle form submission here
      },
    },
  };
  </script>
  