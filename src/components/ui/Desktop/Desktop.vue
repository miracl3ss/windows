<script setup lang="ts">
import AppIcon from './Icon.vue'
    const icons = [{
        name: 'My computer',
        icon: 'computer'  
    }, {
        name: 'My computer',
        icon: 'computer'  
    }, {
        name: 'My computer',
        icon: 'computer'  
    }, {
        name: 'My computer',
        icon: 'computer'  
    }, {
        name: 'My computer',
        icon: 'computer'  
    }, {
        name: 'My computer',
        icon: 'computer'  
    }, {
        name: 'My computer',
        icon: 'computer'  
    }, {
        name: 'My computer',
        icon: 'computer'  
    }, {
        name: 'My computer',
        icon: 'computer'  
    }]
</script>

<template>
    <div class="flex flex-col flex-auto flex-wrap content-start  desktop-wrapper">
        <div v-for="icon in icons" class="w-fit p-4" >
            <AppIcon :icon="icon.icon" >{{ icon.name }}</AppIcon>
        </div>
    </div>
</template>
