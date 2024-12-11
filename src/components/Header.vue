<script setup>
    import imgheder from '../assets/img/header-salon.jpg'
</script>
<template>
    <header class="header flex flex-col justify-center items-center text-white">
      <!-- Título del salón -->
      <div class="text-center mb-4">
        <h1 class="text-5xl font-extrabold text-primary mb-2">Sol Chic</h1>
        <h2 class="text-xl font-medium">Salón de belleza</h2>
      </div>
  
      <!-- Descripción del salón -->
      <div class="text-center max-w-4xl px-4 mb-6">
        <p class="text-lg leading-relaxed">
          Bienvenidos a nuestro salón de belleza. Descubre un mundo de belleza y estilo en nuestra página web. Nuestro equipo de profesionales está aquí para realzar tu belleza y resaltar tu personalidad única. Explora nuestros servicios, inspírate en nuestras creaciones y reserva tu cita para vivir una experiencia inolvidable. Te esperamos con los brazos abiertos.
        </p>
      </div>
  
      <!-- Llamado a la acción -->
        <div class="my-6">
            <a href="#reservar" class="px-8 py-4 text-white bg-gradient-to-r from-purple-500 to-pink-500 hover:bg-gradient-to-l focus:ring-4 focus:outline-none focus:ring-purple-200 dark:focus:ring-purple-800 font-medium rounded-lg text-xl text-center me-2 mb-2">
                Reserva ahora
            </a>
        </div>
    </header>
  </template>
  
<style scoped>
.header {
    background-image: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url('../assets/img/header-salon.jpg');
    width: 100%;
    height: 600px;
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
}
</style>
