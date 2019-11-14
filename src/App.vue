<template>
  <div id="app">
    <AppHero></AppHero>
    <AppServices></AppServices>
    <AppEmployees></AppEmployees>
    <AppArticle></AppArticle>
    <AppKontakt></AppKontakt>
  </div>
</template>

<script>
  import AppHero from "./components/layout/AppHero.vue";
  import AppServices from "./components/scenes/AppServices.vue";
  import AppEmployees from  "./components/scenes/AppEmployees.vue";
  import AppArticle from "./components/scenes/AppArticle";
  import AppKontakt from "./components/scenes/AppKontakt";

  export default {
    components: {
      AppHero,
      AppServices,
      AppEmployees,
      AppArticle,
      AppKontakt
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