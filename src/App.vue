<template>
  <div id="app">
    <NavigationBar />
    <block_first />
    <block_two />
    <router-view />
  </div>
</template>

<script>
import NavigationBar from './components/NavigationBar.vue';
import block_first from "./components/block_1.vue";
import block_two from "./components/block_2";

export default {
  name: 'App',
  components: {
    NavigationBar,
    block_first,
    block_two
  }
};
</script>

<style>
body {
  font-family: 'Roboto', sans-serif;
}
</style>
