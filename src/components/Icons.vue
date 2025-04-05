<script>

import IconMyComputer from '../../public/windows98icons/computer.png'

const icons = {
    computer: IconMyComputer,
    
}
export default {}
</script>

<script setup>
import { computed } from 'vue'

const props = defineProps({
    icon: {
        type: String,
        required: true,
        validator(value) {
            return Object.prototype.hasOwnProperty.call(icons, value)
        },
    },
})

const iconComponent = computed(() => {
    return icons[props.icon]
})
</script>
<template>
    <component :is="iconComponent"></component>
</template>
