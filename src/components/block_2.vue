<template>
  <div class="block_2 bg-background p-4 flex justify-center items-center">
    <Card_1
        image="/pic/card/card_1.png"
        title="Fig. 1 (plant)"
        description="Имеется спорная точка зрения, гласящая примерно следующее: активно развивающиеся страны третьего мира своевременно верифицированы."
        number="2.4"
    />
  </div>
</template>

<script>
import Card_1 from '../components/card/card_1.vue';

export default {
  name: 'block_2',
  components: {
    Card_1
  }
};
</script>

<style scoped>
.block_2 {
  height: auto;
  background-color: #1D2F30;
}

</style>
