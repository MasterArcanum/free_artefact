<template>
  <div class="block_2 bg-gray-900 p-4 flex justify-center items-center">
    <Card_1
        class="Card_1"
        image="/pic/card/card_1.png"
        title="Fig. 1 (plant)"
        description="Имеется спорная точка зрения, гласящая примерно следующее: активно развивающиеся страны третьего мира своевременно верифицированы."
        number="2.4"
    />
    <Card_2
        class="Card_2"
        image="/pic/card/card_2.png"
        title="Fig. 2 (flower)"
        description="Прежде всего, синтетическое тестирование влечет за собой процесс внедрения и модернизации условий."
        number="2.4"
    />
  </div>
</template>

<script>
import Card_1 from '../components/card/card_1.vue';
import Card_2 from '../components/card/card_2.vue';

export default {
  name: 'block_2',
  components: {
    Card_1,
    Card_2
  }
};
</script>

<style scoped>
.block_2 {
  height: auto;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.Card_1, .Card_2 {
  margin: 2rem;
  width: 300px; /* Задаем фиксированную ширину */
  height: 400px; /* Задаем фиксированную высоту */
}
</style>
