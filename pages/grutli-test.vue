<template>
    <section
        class="v-grutli-test"
    >
        <app-nav/>
        <AppHeader/>
    </section>
</template>





<script setup lang="ts">
import { defineProps } from 'vue'
import AppHeader from "~/components/grutli/AppHeader.vue";
import AppNav from "~/components/grutli/AppNav.vue";

const props = defineProps<{
    message?: string
}>()
</script>





<style lang="scss" scoped >
.v-grutli-test {
    font-size: 1rem;
}
</style>
