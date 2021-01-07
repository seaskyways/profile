<template>
  <v-app>
    <v-app-bar app color="primary" dense>
      <v-app-bar-title>Ahmad Al-Sharif's Profile</v-app-bar-title>
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
