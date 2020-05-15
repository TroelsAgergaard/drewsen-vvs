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
import Vue from "vue";
import vueMq from "vue-mq";

Vue.use(vueMq, {
  breakpoints: {
    sm: 768,
    lg: Infinity
  }
});

import AppHero from "./components/layout/AppHero.vue";
import AppServices from "./components/scenes/AppServices.vue";
import AppEmployees from "./components/scenes/AppEmployees.vue";
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
html {
  scroll-behavior: smooth;
}
#app {
  font-family: "Roboto", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #fff;
  h1:not(.header__title) {
    margin: 0 0 3.5rem 0;
    font-size: calc(2.6rem + 1vw);
    line-height: 2.8rem;
  }
}
</style>
