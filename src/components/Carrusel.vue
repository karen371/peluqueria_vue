<script setup>
    import Card from '../components/Card.vue';
    import { ref, onMounted } from 'vue';
    const productos = ref([]);

// Función para obtener los datos desde el archivo JSON
const fetchProductos = async () => {
  try {
    const response = await fetch('http://localhost:3000/productos'); // Cambia la ruta si tu archivo está en otro lugar
    if (!response.ok) {
      throw new Error('Error al cargar los datos');
    }
    productos.value = await response.json();
  } catch (error) {
    console.error('Error al realizar el fetch:', error);
  }
};

// Cargar los datos cuando el componente se monte
onMounted(() => {
  fetchProductos();
});
</script>
<template>
    <div class="carousel carousel-center bg-neutral rounded-box max-w-md space-x-4 p-4 flex">
        <div class="carousel-item">
          <img
            src="https://img.daisyui.com/images/stock/photo-1559703248-dcaaec9fab78.webp"
            class="rounded-box" />
        </div>
        <div class="carousel-item">
          <img
            src="https://img.daisyui.com/images/stock/photo-1565098772267-60af42b81ef2.webp"
            class="rounded-box" />
        </div>
        <div class="carousel-item">
          <img
            src="https://img.daisyui.com/images/stock/photo-1572635148818-ef6fd45eb394.webp"
            class="rounded-box" />
        </div>
      </div>
</template>
<style scoped>

</style>