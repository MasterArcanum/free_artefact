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


<!--макет-->
<!--https://www.figma.com/design/fG61Ja1ye0jtkKbuvt9OR0/Коллекция-природных-артефактов?node-id=13-0&t=PIaZW6LKK3p8s2vt-0-->