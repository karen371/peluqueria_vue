<script setup>
    import imgheder from '../assets/img/header-salon.jpg'

</script>
<template>
    <header class="header text-white">
      <!-- Título del salón -->
      <div class="header-titulo">
          <h1 class="text-5xl font-extrabold text-primary mb-2">Descubre Tu Estilo</h1>
          <h2 class="underline text-2xl  text-primary mb-2">Explora nuestra tienda</h2>
          <button type="button" class="text-white bg-gradient-to-r from-pink-400 via-pink-500 to-pink-600 hover:bg-gradient-to-br focus:ring-4 focus:outline-none focus:ring-pink-300 dark:focus:ring-pink-800 font-medium rounded-lg text-sm px-5 py-2.5 text-center me-2 mb-2">
            Contactanos</button>
      </div>
    </header>
  </template>
  
<style scoped>
.header {
    background-image: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url('../assets/img/header-salon.jpg');
    width: 100%;
    height: 500px;
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    display: flex;
}
.header-titulo {
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
.titulo{
  display: flex;
  flex-direction: column;
}
</style>
