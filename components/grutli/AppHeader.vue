<template>
    <section
        class="v-app-header"
    >
        Scène du Grütli
    </section>
</template>





<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps<{
    message?: string
}>()
</script>





<style lang="scss" scoped >
.v-app-header {
}
</style>
