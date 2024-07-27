<template>
  <div class="card bg-background p-4 rounded-lg shadow-md">
    <div class="relative image_card bg-gray-900 rounded-t-lg">
      <img :src="image" alt="Image" class="rotated-img object-cover py-6">
      <div
          class="absolute top-2 left-2 bg-gray-700 text-white rounded-full w-8 h-8 flex items-center justify-center text-sm">
        {{ number }}
      </div>
    </div>
    <h3 class="text-white font-cormorant text-xl font-bold mb-2">{{ title }}</h3>
    <p class="text-white font-open-sans text-sm mb-4">{{ description }}</p>
    <button class="btn-primary mt-5">
      Подробнее
    </button>
  </div>
</template>

<script>
export default {
  name: 'Card_2',
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
.image_card {
  height: 11rem;
}

.card {
  background-color: #1D2F30;
  max-width: 270px;
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
  background-color: #166401;
}

.text-sm {
  font-size: 0.875rem;
}

.rotated-img {
  transform: rotate(180deg);
  width: 204px;
  height: 120px;
  top: 640px;
  left: 964px;
  gap: 0px;

  margin: 0 auto;
  opacity: 0px;
  angle: -90 deg;

}
</style>
