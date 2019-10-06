<template>
  <div id="app">
    <hero></hero>
    <service></service>
    <employees></employees>
  </div>
</template>

<script>
import Hero from "./components/presentational/Hero.vue";
import Service from "./components/presentational/Service.vue";
import Employees from  "./components/scenes/default.vue";

export default {
  components: {
    Hero,
    Service,
    Employees
  }
};
</script>

<style lang="scss">
#app {
  font-family: 'Roboto', sans-serif;
  font-size: 1.6rem;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #fff;
}
h1{
  margin: 0;
}
</style>