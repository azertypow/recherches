<template>
    <div class="v-app-video-mask"></div>
</template>





<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps<{
    message?: string
}>()
</script>





<style lang="scss" scoped >
.v-app-video-mask {
    display: block;
    width: 100%;
    height: 100%;
    padding: 0;
    background-image: url(https://images.unsplash.com/photo-1528287942171-fbe365d1d9ac?ixlib=rb-1.2.1&q=85&fm=jpg&crop=entropy&w=1200&cs=srgb&ixid=eyJhcHBfaWQiOjE0NTg5fQ);
    background-size: cover;
    background-position: center;
    mask-mode: luminance;
    //mask-repeat: no-repeat;

    mask-image: url('@/assets/Substitution-du-Chrome-decoratif-brillant-Version-francaise-et-anglaise.jpeg');
}
</style>
