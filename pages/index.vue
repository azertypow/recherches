<template>
    <section
        class="v-index"
    >
        <div style="width: 100vw; height: 100vh">
            <AppVideoMask/>
            <AppVideoMask2/>
            <AppTypoGruttli2/>
            <AppVideoMask3/>
            <AppVideoMask4/>
            <AppVideoMask5/>
            <AppVideoMask6/>
            <AppVideoMask7/>
            <AppTypoGruttli/>
            <AppVideoMask00/>
            <AppTypoGruttli3/>
        </div>
    </section>
</template>





<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps<{
    message?: string
}>()
</script>





<style lang="scss" scoped >
.v-index {
}
</style>
