<template>
  <div class="block-1 bg-cover bg-center text-left relative flex items-center justify-start p-8" :style="{ backgroundImage: `url(${backgroundImage})` }">
    <div class="absolute inset-0 bg-black opacity-70"></div>
    <div class="block-1_text relative z-10 max-w-3xl">
      <h1 class="text-white font-open-sans text-6xl  leading-none mb-4">
        Крупнейшая коллекция природных артефактов
      </h1>
      <p class="text-white font-open-sans text-base font-normal leading-6 mb-4">
        Являясь всего лишь частью общей картины, интерактивные прототипы, которые представляют собой яркий пример европейского типа политической и социальной культуры.
      </p>
      <button class="text-primary-green font-open-sans text-base font-bold leading-6 flex items-center">
        Исследовать
        <svg class="ml-2 h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3" />
        </svg>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Block_1',
  data() {
    return {
      backgroundImage: require('@/../public/pic/block_1.png')
    };
  }
};
</script>

<style scoped>
.block-1 {
  width: 100%;
  max-width: 1920px;
  height: 550px;
  gap: 0;
  background-size: cover;
  background-position: center;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: flex-start;
}

.block-1_text {
  margin-left: 300px;
}

.font-cormorant {
  font-family: 'Cormorant', serif;
}

.font-open-sans {
  font-family: 'Open Sans', sans-serif;
}

.text-primary-green {
  color: #BAE249;
}

@media (max-width: 1200px) {
  .block-1_text {
    margin-left: 150px;
  }

  .block-1 h1 {
    font-size: 4rem;
  }
}

@media (max-width: 768px) {
  .block-1 {
    justify-content: center;
    text-align: center;
    padding-left: 0;
  }

  .block-1_text {
    margin-left: 0;
    padding: 0 20px;
  }

  .block-1 h1 {
    font-size: 3rem;
    margin-left: 0;
    margin-right: 0;
  }

  .block-1 p {
    font-size: 1rem;
    margin-left: 0;
    margin-right: 0;
  }

  .block-1 button {
    margin-left: 0;
    margin-right: 0;
  }
}

@media (max-width: 480px) {
  .block-1 {
    height: auto;
    padding: 20px;
  }

  .block-1 h1 {
    font-size: 2rem;
  }

  .block-1 p {
    font-size: 0.875rem;
  }

  .block-1 button {
    font-size: 0.875rem;
  }
}
</style>
