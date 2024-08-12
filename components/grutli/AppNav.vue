<template>
    <section
        class="v-app-nav"
    >
        <div>logo</div>
    </section>
</template>





<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps<{
    message?: string
}>()
</script>





<style lang="scss" scoped >
.v-app-nav {

}
</style>
