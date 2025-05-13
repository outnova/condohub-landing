<template>
  <div class="bg-gray-100 font-sans antialiased">
    <TheNavbar />

    <TheCarousel />

    <section id="inicio" class="py-20 bg-white">
      <div class="container mx-auto px-4">
        <h2 class="text-3xl font-bold text-gray-800 mb-6">Bienvenido a nuestro Sistema de Condominios</h2>
        <p class="text-lg text-gray-600 mb-8">
          La solución integral para la gestión eficiente y transparente de tu condominio.
          Descubre cómo podemos simplificar tu vida y la de tus vecinos.
        </p>
        <button class="bg-indigo-500 hover:bg-indigo-700 text-white font-bold py-3 px-6 rounded-full">
          Conoce más
        </button>
      </div>
    </section>

    <section id="nosotros" class="py-20 bg-gray-100">
      <div class="container mx-auto px-4">
        <h2 class="text-3xl font-bold text-gray-800 mb-6">Nosotros</h2>
        <p class="text-lg text-gray-600">
          Somos un equipo apasionado por la tecnología y la gestión de propiedades.
          Nuestro objetivo es ofrecer una plataforma intuitiva y poderosa que facilite la comunicación,
          la administración y la transparencia en los condominios.
        </p>
        </div>
    </section>

    <section id="servicios" class="py-20 bg-white">
      <div class="container mx-auto px-4">
        <h2 class="text-3xl font-bold text-gray-800 mb-6">Nuestros Servicios</h2>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <div class="bg-white rounded-lg shadow-md p-6">
            <h3 class="text-xl font-semibold text-indigo-600 mb-2">Gestión de Pagos</h3>
            <p class="text-gray-600">Automatiza la recaudación de cuotas y realiza un seguimiento detallado de los pagos.</p>
          </div>
          <div class="bg-white rounded-lg shadow-md p-6">
            <h3 class="text-xl font-semibold text-indigo-600 mb-2">Comunicación Centralizada</h3>
            <p class="text-gray-600">Mantén a todos los residentes informados a través de anuncios, foros y mensajes directos.</p>
          </div>
          <div class="bg-white rounded-lg shadow-md p-6">
            <h3 class="text-xl font-semibold text-indigo-600 mb-2">Reservas de Áreas Comunes</h3>
            <p class="text-gray-600">Facilita la reserva de espacios comunes como salones de eventos, parrilleras, etc.</p>
          </div>
          </div>
      </div>
    </section>

    <section id="clientes" class="py-20 bg-gray-100">
      <div class="container mx-auto px-4">
        <h2 class="text-3xl font-bold text-gray-800 mb-6">Nuestros Clientes</h2>
        <div class="grid grid-cols-2 md:grid-cols-4 gap-8">
          <div class="bg-white rounded-lg shadow-md p-4 flex items-center justify-center">
            <img src="https://placehold.co/100" alt="Cliente 1" class="w-20 h-20 object-contain">
          </div>
          <div class="bg-white rounded-lg shadow-md p-4 flex items-center justify-center">
            <img src="https://placehold.co/100" alt="Cliente 2" class="w-20 h-20 object-contain">
          </div>
          <div class="bg-white rounded-lg shadow-md p-4 flex items-center justify-center">
            <img src="https://placehold.co/100" alt="Cliente 3" class="w-20 h-20 object-contain">
          </div>
          <div class="bg-white rounded-lg shadow-md p-4 flex items-center justify-center">
            <img src="https://placehold.co/100" alt="Cliente 4" class="w-20 h-20 object-contain">
          </div>
          </div>
      </div>
    </section>

    <section id="contacto" class="py-20 bg-white">
      <div class="container mx-auto px-4">
        <h2 class="text-3xl font-bold text-gray-800 mb-6">Contáctanos</h2>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
          <div>
            <p class="text-lg text-gray-600 mb-4">
              ¿Tienes alguna pregunta o deseas solicitar una demostración? ¡No dudes en contactarnos!
            </p>
            <ul class="list-none space-y-2">
              <li class="flex items-center">
                <svg class="w-5 h-5 mr-2 text-gray-500" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8m-7 2h4m-7 0h-4m-3 5h4m-7 0h-4m-9-5h2m5-1V9m0 1v5m0 5H9m3 0h3m-3-3h3m-3-3h3"></path></svg>
                info@misistema.com
              </li>
              <li class="flex items-center">
                <svg class="w-5 h-5 mr-2 text-gray-500" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h14a2 2 0 012 2v14a2 2 0 01-2 2H5a2 2 0 01-2-2V5z"></path></svg>
                +58 414 123 4567
              </li>
              <li class="flex items-center">
                <svg class="w-5 h-5 mr-2 text-gray-500" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0L6.343 16.657a9 9 0 1111.314 0z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"></path></svg>
                Coro, Falcón, Venezuela
              </li>
            </ul>
          </div>
          <div>
            <form class="space-y-4">
              <div>
                <label for="nombre" class="block text-gray-700 text-sm font-bold mb-2">Nombre</label>
                <input type="text" id="nombre" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" placeholder="Tu nombre">
              </div>
              <div>
                <label for="email" class="block text-gray-700 text-sm font-bold mb-2">Email</label>
                <input type="email" id="email" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" placeholder="Tu correo electrónico">
              </div>
              <div>
                <label for="mensaje" class="block text-gray-700 text-sm font-bold mb-2">Mensaje</label>
                <textarea id="mensaje" rows="4" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" placeholder="Escribe tu mensaje"></textarea>
              </div>
              <button type="submit" class="bg-indigo-500 hover:bg-indigo-700 text-white font-bold py-3 px-6 rounded-full focus:outline-none focus:shadow-outline">
                Enviar mensaje
              </button>
            </form>
          </div>
        </div>
      </div>
    </section>

    <TheFooter />
  </div>
</template>

<script>
import TheNavbar from './components/TheNavbar.vue';
import TheCarousel from './components/TheCarousel.vue';
import TheFooter from './components/TheFooter.vue';

export default {
  components: {
    TheNavbar,
    TheCarousel,
    TheFooter,
  },
  mounted() {
    // Implementación del scroll suave al hacer clic en los enlaces del navbar
    const navLinks = document.querySelectorAll('nav a');
    navLinks.forEach(link => {
      link.addEventListener('click', function(event) {
        event.preventDefault();
        const targetId = this.getAttribute('href');
        const targetElement = document.querySelector(targetId);
        if (targetElement) {
          window.scrollTo({
            top: targetElement.offsetTop,
            behavior: 'smooth'
          });
        }
      });
    });
  }
}
</script>