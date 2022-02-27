<template>
  <v-app>
    <core-layout />
  </v-app>
</template>

<script>
import CoreLayout from "./components/core/Layout.vue";

export default {
  name: "App",
  components: {
    CoreLayout,
  },
  data: () => ({}),
};
</script>
