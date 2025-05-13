<template>
    <div class="relative">
      <div class="overflow-hidden relative w-full">
        <div 
          class="transition-transform duration-500 ease-in-out flex" 
          :style="{ transform: `translateX(-${currentIndex * 100}%)` }"
        >
          <div 
            v-for="(slide, index) in slides" 
            :key="index" 
            class="w-full flex-shrink-0 relative"
          >
            <img 
              :src="slide.image" 
              :alt="slide.alt" 
              class="w-full h-96 object-cover"
            >
            <div class="absolute bottom-0 left-0 w-full bg-black bg-opacity-50 text-white p-4">
              <h3 class="text-xl font-semibold">{{ slide.title }}</h3>
              <p class="text-sm">{{ slide.description }}</p>
            </div>
          </div>
        </div>
      </div>
      <button 
        @click="prevSlide" 
        class="absolute top-1/2 left-4 transform -translate-y-1/2 bg-gray-800 bg-opacity-50 text-white rounded-full p-2 focus:outline-none"
      >
        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7" />
        </svg>
      </button>
      <button 
        @click="nextSlide" 
        class="absolute top-1/2 right-4 transform -translate-y-1/2 bg-gray-800 bg-opacity-50 text-white rounded-full p-2 focus:outline-none"
      >
        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
        </svg>
      </button>
    </div>
  </template>
  
  <script>
  import { ref, onMounted, onUnmounted } from 'vue';
  
  export default {
    setup() {
      const currentIndex = ref(0);
      const slides = ref([
        { image: 'https://placehold.co/1200/4A5568/FFFFFF?Text=Slide%201', title: 'Gestión Eficiente', description: 'Optimiza la administración de tu condominio.' },
        { image: 'https://placehold.co/1200/2C3E50/FFFFFF?Text=Slide%202', title: 'Comunicación Clara', description: 'Mantén a todos informados y conectados.' },
        { image: 'https://placehold.co/1200/34495E/FFFFFF?Text=Slide%203', title: 'Reservas Sencillas', description: 'Gestiona las áreas comunes de forma intuitiva.' },
      ]);
      const intervalId = ref(null);
      const slideCount = slides.value.length;
  
      const nextSlide = () => {
        currentIndex.value = (currentIndex.value + 1) % slideCount;
      };
  
      const prevSlide = () => {
        currentIndex.value = (currentIndex.value - 1 + slideCount) % slideCount;
      };
  
      const startAutoplay = () => {
        intervalId.value = setInterval(nextSlide, 5000); // Cambia de slide cada 5 segundos
      };
  
      const stopAutoplay = () => {
        clearInterval(intervalId.value);
      };
  
      onMounted(() => {
        startAutoplay();
      });
  
      onUnmounted(() => {
        stopAutoplay();
      });
  
      return {
        currentIndex,
        slides,
        nextSlide,
        prevSlide,
      };
    },
  }
  </script>