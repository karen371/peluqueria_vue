<script setup>
import { ref } from 'vue';
import imglogo from '../assets/img/logo2.png';

const menuOpen = ref(false);

function toggleMenu() {
  menuOpen.value = !menuOpen.value;
}
</script>
<template>
  <nav class="w-full z-50 top-0 start-0 border-b border-gray-200 nav">
    <div
      class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4"
    >
      <!-- Logo -->
      <span class="flex items-center space-x-3 rtl:space-x-reverse">
        <img :src="imglogo" class="h-20" alt="sol chic logo" />
      </span>
      
      <!-- Botón de responsividad -->
      <button
        class="inline-flex items-center p-2 w-10 h-10 justify-center text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200"
        aria-controls="navbar-sticky"
        aria-expanded="false"
        @click="toggleMenu"
      >
        <span class="sr-only">Abrir menú</span>
        <svg class="w-5 h-5" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
        </svg>
      </button>

      <!-- Menú -->
      <div
        :class="['items-center justify-between w-full md:flex md:w-auto md:order-1', { hidden: !menuOpen }]"
        id="navbar-sticky"
      >
        <ul
          class="flex flex-col p-4 md:p-0 mt-4 font-medium border md:space-x-8 rtl:space-x-reverse md:flex-row md:mt-0 md:border-0"
        >
          <li>
            <a
              href="#"
              class="block py-2 px-3 text-primary rounded md:bg-transparent md:p-0"
              aria-current="page"
              >El Salón</a
            >
          </li>
          <li>
            <a
              href="#"
              class="block py-2 px-3 text-primary rounded hover:bg-gray-100 md:hover:bg-transparent md:p-0"
              >Servicios</a
            >
          </li>
          <li>
            <a
              href="#"
              class="block py-2 px-3 text-primary rounded hover:bg-gray-100 md:hover:bg-transparent md:p-0"
              >Novias</a
            >
          </li>
          <li>
            <a
              href="#"
              class="block py-2 px-3 text-primary rounded hover:bg-gray-100 md:hover:bg-transparent md:p-0"
              >Tienda</a
            >
          </li>
          <li>
            <a
              href="#"
              class="block py-2 px-3 text-primary rounded hover:bg-gray-100 md:hover:bg-transparent md:p-0"
              >Horarios y Locales</a
            >
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>
<style scoped>
.nav {
  background-color: var(--vt-c-black);
}

.text-primary {
  color: var( --vt-c-white-mute); /* Usando un color definido */
}

.text-primary:hover {
  color: var(--color-heading); /* Cambia al rosa vibrante en hover */
}
</style>
