<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <base-header />
    <the-main />

    <base-footer />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import BaseHeader from "./components/BaseHeader.vue";
import TheMain from "./components/TheMain.vue";
import BaseFooter from "./components/BaseFooter.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    BaseHeader,
    TheMain,
    BaseFooter,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
