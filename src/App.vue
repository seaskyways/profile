<template>
  <v-app>
    <v-app-bar app color="primary" dense>
      <v-app-bar-title>Ahmad Al-Sharif's Profile</v-app-bar-title>
      <v-spacer />
      <v-btn
        href="https://github.com/seaskyways/profile"
        target="_blank"
        depressed
      >
        <v-icon class="me-1">mdi-github</v-icon> Github
      </v-btn>
    </v-app-bar>
    <v-main class="teal lighten-2">
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",
  components: {},
  data: () => ({
    tab: 0
    //
  })
};
</script>

<style></style>
