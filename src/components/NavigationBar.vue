<template>
  <nav class="bg-gray-800 shadow-md">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between h-16">
        <div class="flex items-center">
          <img class="h-12 w-24" src="logo.png" alt="Logo">
          <div class="hidden md:block mx-6">
            <div class="ml-10 flex items-baseline space-x-4">
              <a href="#" class="text-gray-200 hover:text-gray-400  block px-6 py-2 rounded-md text-base font-medium">Каталог</a>
              <a href="#" class="text-gray-200 hover:text-gray-400  block px-6 py-2 rounded-md text-base font-medium">Галерея</a>
              <a href="#" class="text-gray-200 hover:text-gray-400  block px-6 py-2 rounded-md text-base font-medium">О лаборатории</a>
              <a href="#" class="text-gray-200 hover:text-gray-400  block px-6 py-2 rounded-md text-base font-medium">Контакты</a>
            </div>
          </div>
        </div>
        <div class="hidden md:flex items-center space-x-4">
          <button class="p-1 rounded-full text-primary-green hover:text-white focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-offset-gray-800 focus:ring-white" title="Поиск....">
            <span class="sr-only">Search</span>
            <svg class="h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true" >
              <circle cx="11" cy="11" r="8" stroke="#BAE249" stroke-width="2"></circle>
              <line x1="21" y1="21" x2="16.65" y2="16.65" stroke="#BAE249" stroke-width="2"></line>
            </svg>
          </button>
          <button class="p-1 rounded-full text-primary-green hover:text-white focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-offset-gray-800 focus:ring-white" title="Вход">
            <span class="sr-only">Log in</span>
            <!-- Log in icon -->
            <svg class="h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true" >
              <line x1="3" y1="12" x2="12" y2="12" stroke="#BAE249" stroke-width="2"></line>
              <polyline points="8 6 13 12 8 18" stroke="#BAE249" stroke-width="2" fill="none"></polyline>
              <path d="M15 3h3a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2h-3" stroke="#BAE249" stroke-width="2" fill="none"></path>
            </svg>
          </button>
        </div>
        <div class="-mr-2 flex md:hidden">
          <button @click="toggleMenu" class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-gray-200 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-offset-gray-800 focus:ring-white">
            <span class="sr-only">Open main menu</span>
            <svg class="block h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
            </svg>
          </button>
        </div>
      </div>
    </div>

    <div class="md:hidden" id="mobile-menu" :class="{ 'block': isMenuOpen, 'hidden': !isMenuOpen }">
      <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
        <a href="#" class="text-gray-300 hover:text-gray-200  block px-3 py-2 rounded-md text-base font-medium">Каталог</a>
        <a href="#" class="text-gray-300 hover:text-gray-200  block px-3 py-2 rounded-md text-base font-medium">Галерея</a>
        <a href="#" class="text-gray-300 hover:text-gray-200  block px-3 py-2 rounded-md text-base font-medium">О лаборатории</a>
        <a href="#" class="text-gray-300 hover:text-gray-200  block px-3 py-2 rounded-md text-base font-medium">Контакты</a>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      isMenuOpen: false
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    }
  }
};
</script>

<style scoped>
.text-primary-green {
  color: #BAE249;
}
a{
  font-size: 16px;
}
</style>
