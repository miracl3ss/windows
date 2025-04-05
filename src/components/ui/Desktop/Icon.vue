<script setup lang="ts">
    const props = defineProps({
    // theme: {
    //     type: String,
    //     default: 'action',
    // },
    // size: {
    //     type: String,
    //     default: 'md',
    // },
    icon: {
        type: String,
        default: '',
    },
})

const iconComputed = './windows98icons/' + props.icon + '.png'
</script>

<template>
    <div class="flex flex-col items-center w-fit">
        <img :src="iconComputed" class="py-1">
        <h1 class="font-sans cursor-pointer text-base py-1 capitalize"><slot></slot></h1>
    </div>
</template>