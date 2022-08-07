<template>
  <HomePage/>
</template>

<script>
import HomePage from "./page/home.vue";

export default {
  name: 'App',
  components: {
    HomePage
}
}
</script>

<style>

@import url('./style/reset.css');
#app {
  font-family: 'Roboto', sans-serif;
}
</style>
