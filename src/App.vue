<template>
  <div id="app">
    <core-layout></core-layout>
  </div>
</template>

<script>
import CoreLayout from "./components/core/Layout.vue";

export default {
  name: "App",

  components: {
    CoreLayout,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
