<template>
    <div @mousemove="updateMousePosition"
         class="v-app-video-mask4"
    >
        <div class="gruttli">exemple</div>
        <div
            class="v-app-video-mask4--mask"
             :style="{
             }"
        >
            mask4
            <div>{{mousePosition.x}}
                <br>{{mousePosition.y}}
                <br>{{mousePosition.screenPercentPositionX}}
                <br>{{mousePosition.screenPercentPositionY}}
            </div>
        </div>
    </div>
</template>





<script setup lang="ts">

import type {UnwrapNestedRefs} from "vue";

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
.v-app-video-mask4 {
    position: relative;
    width: 100%;
    height: 100%;
}

.v-app-video-mask4--mask {
    width: 100%;
    height: 100%;
    display: block;
    padding: 0;
    background-image: url(https://images.unsplash.com/photo-1528287942171-fbe365d1d9ac?ixlib=rb-1.2.1&q=85&fm=jpg&crop=entropy&w=1200&cs=srgb&ixid=eyJhcHBfaWQiOjE0NTg5fQ);
    background-size: cover;
    background-position: center;
    mask-mode: luminance;
    mask-repeat: no-repeat;
    mask-size: 100% 100%;
    mask-image: url('@/assets/Substitution-du-Chrome-decoratif-brillant-Version-francaise-et-anglaise.jpeg');
}


.gruttli {
    font-size: calc(2083.3vw / 100);
    line-height: 1em;
    font-variation-settings:
        'TRIP' 1;
    position: absolute;
    bottom: 0;
}
</style>
