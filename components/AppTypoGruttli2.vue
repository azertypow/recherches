<template>
    <section
        class="v-app-typo-gruttli"
        @mousemove="updateMousePosition"
        :style="{
            fontVariationSettings: `'TRIP' ${mousePosition.screenPercentPositionX}`
        }"
    >
        scènes
        <br>&emsp;du&nbsp;Grütli
        <br>
        <br>
        <br>
        <br>scènes
        <br>&nbsp;du&nbsp;Grütli
        <br>
        <br>
        <br>Scènes
        <br>&nbsp;du&nbsp;Grütli
        <br>
        <br>
        <br>scènes&emsp;du&nbsp;Grütli
    </section>
</template>



<!--
&emsp;
&nbsp;
-->

<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps<{
    message?: string
}>()

const mousePosition = reactive({
    x: 0,
    y: 0,
    screenPercentPositionX: 0,
    screenPercentPositionY: 0,
})

function updateMousePosition(e: MouseEvent) {
    mousePosition.x = e.x
    mousePosition.y = e.y
    mousePosition.screenPercentPositionX = e.x / window.innerWidth
    mousePosition.screenPercentPositionY = e.y / window.innerHeight
}
</script>





<style lang="scss" scoped >
.v-app-typo-gruttli {
    font-size: calc(208.3vw / 100);
    line-height: 1em;
    font-variation-settings:
            'TRIP' 1
    ;
}
</style>
