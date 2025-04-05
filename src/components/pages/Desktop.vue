<script setup lang="ts">
import DesktopBar from '../ui/Desktop/Bar.vue';
import Desktop from '../ui/Desktop/Desktop.vue';

</script>

<template>
<main>
    <Desktop />
    <DesktopBar />
</main>
</template>

<style scoped>
main {
    background-color: #008081;
    height: 100vh;
    width: 100vw;
}
</style>