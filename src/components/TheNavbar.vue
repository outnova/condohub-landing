<template>
    <nav class="bg-white shadow-md py-4">
      <div class="container mx-auto px-4 flex items-center justify-between">
        <div class="flex items-center">
          <img src="../assets/logo.png" alt="Logo" class="h-8 mr-4">
          <span class="font-bold text-xl text-indigo-600">Tu Sistema</span>
        </div>
        <div class="hidden md:flex space-x-6">
          <a href="#inicio" class="text-gray-700 hover:text-indigo-500">Inicio</a>
          <a href="#nosotros" class="text-gray-700 hover:text-indigo-500">Nosotros</a>
          <a href="#servicios" class="text-gray-700 hover:text-indigo-500">Servicios</a>
          <a href="#clientes" class="text-gray-700 hover:text-indigo-500">Clientes</a>
          <a href="#contacto" class="text-gray-700 hover:text-indigo-500">Contacto</a>
        </div>
        <div class="md:hidden">
          <button @click="toggleMenu" class="text-gray-500 hover:text-indigo-500 focus:outline-none focus:ring-2 focus:ring-indigo-500">
            <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
            </svg>
          </button>
        </div>
      </div>
  
      <div v-if="isMenuOpen" class="md:hidden bg-gray-100 shadow-md mt-2 py-2 rounded">
        <a href="#inicio" class="block py-2 px-4 text-gray-700 hover:bg-indigo-100 hover:text-indigo-500">Inicio</a>
        <a href="#nosotros" class="block py-2 px-4 text-gray-700 hover:bg-indigo-100 hover:text-indigo-500">Nosotros</a>
        <a href="#servicios" class="block py-2 px-4 text-gray-700 hover:bg-indigo-100 hover:text-indigo-500">Servicios</a>
        <a href="#clientes" class="block py-2 px-4 text-gray-700 hover:bg-indigo-100 hover:text-indigo-500">Clientes</a>
        <a href="#contacto" class="block py-2 px-4 text-gray-700 hover:bg-indigo-100 hover:text-indigo-500">Contacto</a>
      </div>
    </nav>
  </template>
  
  <script>
  import { ref } from 'vue';
  
  export default {
    setup() {
      const isMenuOpen = ref(false);
  
      const toggleMenu = () => {
        isMenuOpen.value = !isMenuOpen.value;
      };
  
      return {
        isMenuOpen,
        toggleMenu,
      };
    },
  }
  </script>