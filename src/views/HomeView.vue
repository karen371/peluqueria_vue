<script setup>
import Navbar from '../components/Navbar.vue'
import Header from '@/components/Header.vue';
</script>

<template>
  <header class="flex flex-col">
    <Navbar/>
    <Header/>
  </header>
  <main>
    <section class="container mx-auto p-8 bg-gray-200 flex flex-col">
      <div class="flex flex-col items-center">
        <h2 class="text-3xl font-extrabold text-primary mb-2">Te puede interesar</h2>
      </div>
      <div class="container mx-auto p-8 flex flex-row justify-center space-x-4">
        <div class="flip-container ">
          <div class="card">
            <div class="front absolute inset-0 bg-cover bg-center" style="background-image: url('https://kuchisalon.com/wp-content/uploads/2022/12/cabello_category.jpg');">
            </div>
            <div class="back absolute inset-0 bg-cover bg-center" style="background-image: url('https://kuchisalon.com/wp-content/uploads/2022/12/cabello_category.jpg');">
              <p class="">CORTE</p>
            </div>
          </div>
        </div> 
      </div>
    </section>
    <section>
      <!--Servicios-->
    </section>
    <section>
      <!--Productos utilizados-->
    </section>
    <section>
      <!--Tratamientos-->
    </section>
    <section>
      <!--Promociones-->
    </section>
    <section>
      <!--Contacto-->
    </section>

  </main>

</template>
<style scoped>

.flip-container {
  background-color: transparent;
  width: 400px;
  height: 400px;
  perspective: 1000px; 
}
.card {
  position: relative;
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 1s;
  transform-style: preserve-3d;
}
.flip-container:hover .card {
  transform: rotateY(180deg);
}
.front, .back {
  position: absolute;
  width: 100%;
  height: 100%;
  backface-visibility: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 5rem;
}

.back {
  font-size: 3rem;
  color: var(--color-heading);
  transform: rotateY(180deg);
}
</style>
