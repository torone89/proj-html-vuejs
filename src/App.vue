<template>
  <div id="app">
    <base-header />
    <the-main />
    <base-footer :footerInfo="footerInfo" />
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
  data() {
    return {
      footerInfo: {
        name: "Avada Barbers",
        address: "123 New York Street",
        city: "New York City",
        email: "info@yourwebsite.com",
        number: "+1 (555) 555-1212",
      },
    };
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>
