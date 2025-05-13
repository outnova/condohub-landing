<template>
    <footer class="bg-gray-800 text-white py-8">
      <div class="container mx-auto px-4 text-center">
        <p class="mb-2">
          <strong class="text-indigo-400">Tu Sistema de Condominios</strong> | Todos los derechos reservados &copy; {{ currentYear }}
        </p>
        <nav class="space-x-4">
          <a href="#" class="text-gray-300 hover:text-white">Términos y Condiciones</a>
          <a href="#" class="text-gray-300 hover:text-white">Política de Privacidad</a>
        </nav>
      </div>
    </footer>
  </template>
  
  <script>
  import { ref, onMounted } from 'vue';
  
  export default {
    setup() {
      const currentYear = ref(new Date().getFullYear());
      return {
        currentYear,
      };
    },
  }
  </script>