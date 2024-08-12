<template>
    <div class="v-app-video-mask2"
         @mousemove="updateMousePosition"
         :style="{
             maskSize: `calc( 100% + 100% * ${mousePosition.screenPercentPositionX}) calc( 100% + 100% * ${mousePosition.screenPercentPositionY})`
         }"
    >
        mack2
        <div>{{mousePosition.x}}
            <br>{{mousePosition.y}}
            <br>{{mousePosition.screenPercentPositionX}}
            <br>{{mousePosition.screenPercentPositionY}}
        </div>
    </div>
</template>





<script setup lang="ts">

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
.v-app-video-mask2 {
    display: block;
    width: 100%;
    height: 100%;
    padding: 0;
    background-image: url(https://images.unsplash.com/photo-1528287942171-fbe365d1d9ac?ixlib=rb-1.2.1&q=85&fm=jpg&crop=entropy&w=1200&cs=srgb&ixid=eyJhcHBfaWQiOjE0NTg5fQ);
    background-size: cover;
    background-position: center;
    mask-mode: luminance;
    mask-repeat: no-repeat;
    mask-size: 100% 100%;
    mask-image: url('@/assets/Substitution-du-Chrome-decoratif-brillant-Version-francaise-et-anglaise.jpeg');
}
</style>
