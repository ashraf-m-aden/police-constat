
<template>
<header-layout></header-layout>
  <router-view />
<footer-layout></footer-layout>
</template>


<script setup lang="ts">
import HeaderLayout from './layout/HeaderLayout.vue';
import FooterLayout from './layout/FooterLayout.vue';

</script>

<style scoped>

</style>
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
      color: #42b983;
    }
  }
}
</style>
