<template>
  <div class="card bg-background p-4 rounded-lg shadow-md">
    <div class="relative">
      <img :src="image" alt="Image" class="rotated-img w-full h-40 object-cover rounded-t-lg mb-4">
      <div class="absolute top-2 left-2 bg-gray-700 text-white rounded-full w-8 h-8 flex items-center justify-center text-sm">{{ number }}</div>
    </div>
    <h3 class="text-white font-cormorant text-xl font-bold mb-2">{{ title }}</h3>
    <p class="text-white font-open-sans text-sm mb-4">{{ description }}</p>
    <button class="btn-primary">
      Подробнее
    </button>
  </div>
</template>

<script>
export default {
  name: 'Card_1',
  props: {
    image: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: true
    },
    description: {
      type: String,
      required: true
    },
    number: {
      type: String,
      required: true
    }
  }
};
</script>

<style scoped>
.card {
  background: #0B1919;
  max-width: 250px;
}

.font-cormorant {
  font-family: 'Cormorant', serif;
}


.font-open-sans {
  font-family: 'Open Sans', sans-serif;
}

.btn-primary {
  background-color: transparent;
  border: 2px solid #BAE249;
  color: #BAE249;
  padding: 0.5rem 1rem;
  font-size: 1rem;
  font-weight: bold;
  text-align: center;
  transition: background-color 0.3s, color 0.3s;
}

.btn-primary:hover {
  background-color: #BAE249;
  color: #1D2F30;
}

.relative .bg-gray-700 {
  background-color: #2C3E50;
}

.text-sm {
  font-size: 0.875rem;
}

.rotated-img {
  width: 30%;
  margin: 0 auto;
  transform: rotate(90deg); /* Поворот изображения на 90 градусов */
}
</style>
