<template>
  <div class="block_2 bg-gray-900 flex justify-center items-center">
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
        number="3.1"
    />
    <Card_3
        class="Card_3"
        image="/pic/card/card_3.png"
        title="Fig. 3 (leaf)"
        description="Лишь непосредственные участники прогресса неоднозначны и будут в равной степени предоставлены сами себе для работы."
        number="4.2"
    />
    <Card_4
        class="Card_4"
        image="/pic/card/card_4.png"
        title="Fig. 4 (wood)"
        description="Базовый вектор развития не даёт нам иного выбора, кроме определения новых предложений."
        number="4.2"
    />
  </div>
</template>

<script>
import Card_1 from '../components/card/card_1.vue';
import Card_2 from '../components/card/card_2.vue';
import Card_3 from '../components/card/card_3.vue';
import Card_4 from '../components/card/card_4.vue';

export default {
  name: 'block_2',
  components: {
    Card_1,
    Card_2,
    Card_3,
    Card_4
  }
};
</script>

<style scoped>
.block_2 {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  margin: 0 auto;
  padding: 1rem;
}

.Card_1, .Card_2, .Card_3, .Card_4 {
  flex: 1 1 calc(25% - 2rem);
  margin: 1rem;
  width: 250px;
  height: 400px;
}

@media (max-width: 1200px) {
  .Card_1, .Card_2, .Card_3, .Card_4 {
    flex: 1 1 calc(33.33% - 2rem);
  }
}

@media (max-width: 900px) {
  .Card_1, .Card_2, .Card_3, .Card_4 {
    flex: 1 1 calc(50% - 2rem);
  }
}

@media (max-width: 600px) {
  .Card_1, .Card_2, .Card_3, .Card_4 {
    flex: 1 1 100%;
    margin: 0.5rem 0;
  }
}
</style>
