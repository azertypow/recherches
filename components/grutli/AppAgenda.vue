<template>
    <section
        class="v-app-agenda"
    >
        Agenda
        <div>cette semaine</div>
        <div>aujourd'hui</div>
        <div>agenda 1</div>
    </section>
</template>





<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps<{
    message?: string
}>()
</script>





<style lang="scss" scoped >
.v-app-agenda {
}
</style>
