<template>
  <app-header></app-header>
  <router-view />
</template>
<script>
import AppHeader from "./components/AppHeader.vue";
export default {
  name: "App",
  components: { AppHeader },
};
</script>
<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #3b0bbe;
    }
  }
}
</style>
