<script setup lang="ts">
import NavBar from './navBar.vue';
import Footer from './footer.vue';
</script>

<template>
    <div>
        <NavBar />
        <slot />
        <Footer />
    </div>
</template>