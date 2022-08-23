<template>
  <div id="app">
    <base-header />
    <the-main />
    <base-footer />
  </div>
</template>

<script>
import BaseHeader from "./components/BaseHeader.vue";
import TheMain from "./components/TheMain.vue";
import BaseFooter from "./components/BaseFooter.vue";

// Import Sass
import "./assets/sass/style.scss";

export default {
  name: "App",
  components: {
    BaseHeader,
    TheMain,
    BaseFooter,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>
