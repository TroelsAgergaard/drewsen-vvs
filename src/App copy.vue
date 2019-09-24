<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <hero></hero>
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Hero from "./components/Hero.vue";

//Er det dennt eksport som bliver auto injected i #app elementet?
export default {
  name: "app",
  components: { // Hvor kan man finde information vedr. components propertis
    HelloWorld,
    Hero
  }
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
