<script>
export default {
    props: {
        producto: {
            type: Object,
            required: true,
        },
    },
};
</script>

<template>
<div v-if="producto" class="max-w-sm bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700">
    <a href="#">
        <img v-if="producto.imagen" class="rounded-t-lg" :src="producto.imagen" :alt="producto.nombre" />
    </a>
    <div class="p-5">
        <a href="#">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">{{ producto.nombre }}</h5>
        </a>
        <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">{{ producto.precio }}</p>
        <button class="px-4 py-2 bg-blue-500 text-white rounded hover:bg-blue-600">
            Agregar al carro
        </button>
    </div>
</div>
</template>
