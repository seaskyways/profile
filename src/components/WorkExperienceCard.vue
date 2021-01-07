<template>
  <v-card tile>
    <v-card-title>
      <div class="d-flex flex-column" style="word-break: normal; width: 100%">
        <v-row no-gutters>
          <v-col cols="12" md class="text-h5">{{ from }} - {{ to }}</v-col>
          <v-col cols="12" md class="text-h6 text-md-end" v-html="workPlace">
          </v-col>
        </v-row>
        <div class="text-md-h2 text-h4">
          {{ title }}
        </div>
      </div>
    </v-card-title>
    <v-card-text>
      <ul class="body-1">
        <li v-for="exp in experiences" :key="exp" v-html="exp"></li>
      </ul>
    </v-card-text>
    <slot name="append"></slot>
  </v-card>
</template>

<script>
export default {
  name: "WorkExperienceCard",
  props: ["from", "to", "title", "workPlace", "experiences"]
};
</script>

<style scoped>
li >>> b {
  color: #63b2ab;
}
</style>
