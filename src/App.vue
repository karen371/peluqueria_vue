<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Navbar from './components/Navbar.vue';
import Header from './components/Header.vue';
</script>

<template>
    <div class="flex flex-col">
        <div><Navbar/></div>
        <div><Header/></div>
    </div>
    <RouterView />
</template>

<style scoped>

</style>
