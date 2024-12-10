<script setup>
import imglogo from '../assets/img/logo.png'

</script>
<template>
  <nav class="fixed w-full z-20 top-0 start-0 border-b border-gray-200 nav">
    <div
      class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4"
    >
      <span class="flex items-center space-x-3 rtl:space-x-reverse">
        <img :src="imglogo" class="h-20" alt="sol chic logo" />
      </span>
      <div
        class="items-center justify-between hidden w-full md:flex md:w-auto md:order-1"
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
              >Inicio</a
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
              >Tratamientos</a
            >
          </li>
          <li>
            <a
              href="#"
              class="block py-2 px-3 text-primary rounded hover:bg-gray-100 md:hover:bg-transparent md:p-0"
              >Promociones</a
            >
          </li>
          <li>
            <a
              href="#"
              class="block py-2 px-3 text-primary rounded hover:bg-gray-100 md:hover:bg-transparent md:p-0"
              >Contacto</a
            >
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<style scoped>
.nav {
  background-color: var(--color-background-soft);
}

.text-primary {
  color: var(--vt-c-text-light-1); /* Usando un color definido */
}

.text-primary:hover {
  color: var(--color-heading); /* Cambia al rosa vibrante en hover */
}
</style>
