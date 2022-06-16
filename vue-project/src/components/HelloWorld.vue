<template>
  <v-layout>
    <v-app-bar color="grey-lighten-2"></v-app-bar>
    <v-main>
      <v-row>
        <v-col
          v-for="item in ecosystem"
          :key="item"
          xs="3"
          sm="3"
          md="3"
          lg="3"
        >
          {{ item }}
        </v-col>
      </v-row>
    </v-main>
  </v-layout>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "HelloWorld",

  data() {
    return {
      ecosystem: [1, 2, 3, 4, 5, 6, 7, 8, 9],
    };
  },
});
</script>
