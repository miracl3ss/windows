<script setup lang="ts">
import { useNow } from '@vueuse/core';

const now = useNow();
</script>
<template>
    <div class="desktop-tray__wrapper">
        <img src="/windows98icons/calendar.png" alt="">
        <img src="/windows98icons/loudspeaker_muted.png" alt="">
        <h1 >{{ now.toLocaleTimeString('ru', { hour: '2-digit', minute: '2-digit' }) }}</h1>
    </div>
</template>

