<template>
    <section
        class="v-app-typo-gruttli"
        @mousemove="updateMousePosition"
        :style="{
            fontVariationSettings: `'TRIP' ${mousePosition.screenPercentPositionX}`
        }"
    >
        <span>s</span>
        <span>c</span>
        <span>è</span>
        <span>n</span>
        <span>e</span>
        <span>s</span>
        <br>&emsp;
        <span>d</span>
        <span>u&nbsp;</span>
        <span>G</span>
        <span>r</span>
        <span>ü</span>
        <span>t</span>
        <span>l</span>
        <span>i</span>
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

span:nth-child(1n) {
    background: red;
}

span:nth-child(2n) {
    background: blue;
}

span:nth-child(3n) {
    background: green;
}
</style>
