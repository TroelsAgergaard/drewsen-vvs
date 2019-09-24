<template>
  <div id="app">
    <hero></hero>
    <service></service>
  </div>
</template>

<script>
import Hero from "./components/presentational/Hero.vue";
import Service from "./components/presentational/Service.vue";

export default {
  components: {
    Hero,
    Service
  }
};
</script>

<style lang="scss">
#app {
  font-family: 'Roboto', sans-serif;
  font-size: 1.6em;  
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
