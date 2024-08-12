<template>
    <section
        class="v-app-typo-gruttli"
    >
        grutli   nnn
    <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ooo
    <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;uuu
    <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;sss
    <br>
    <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;aaa
    <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;vvv
    <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ooo
    <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;nnn
    <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;sss



        <div class="d3-effect">
            <div><div style="transform: rotate3d(0, 1, 0, 0deg)" >scenes</div></div>
            <div><div style="transform: rotate3d(0, 1, 0, 45deg)" >du</div></div>
            <div><div style="transform: rotate3d(0, 1, 0, 0deg)" >Grutli</div></div>
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
.v-app-typo-gruttli {
    font-size: calc(2083.3vw / 100);
    line-height: .65em;
    font-variation-settings:
        'TRIP' 1
    ;
}

.d3-effect {
    position: relative;
    font-size: 5rem;
    line-height: 1em;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    transform: rotate3d(1, 1, 1, -45deg);
    transform-origin: top left;
    perspective: 10000000px;

    > div {
        &:nth-child(2) {
            > div {
                color: black;
                background: white;
            }
        }

        > div {
            transform-origin: left;
            display: inline-block;
            position: relative;
            color: white;
            background: black;
        }
    }
}
</style>
