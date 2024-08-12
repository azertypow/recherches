<template>
    <section
        class="v-animation"
    >
        <div>
            <div class="text" >Scènes du Grütli</div>
            <div class="text" >Scènes du Grütli</div>
            <div class="text" >Scènes du Grütli</div>
            <div class="text" >Scènes du Grütli</div>
            <div class="text" >Scènes du Grütli</div>
            <div class="text" >Scènes du Grütli</div>
            <div class="text" >Scènes du Grütli</div>
            <div class="text" >Scènes du Grütli</div>
            <div class="text" >Scènes du Grütli</div>
            <div class="text" >Scènes du Grütli</div>
        </div>
    </section>
</template>





<script setup lang="ts">

</script>





<style lang="scss" scoped >
.v-animation {
    font-weight: 900;
    font-size: 12.5vw;
    letter-spacing: 0em;
    text-align: center;
}

.text {
    position: fixed;
    top: calc(50% - 2rem);
    left: 50%;
    transform: translate(-50%, -50%);
    width: 100%;
    animation: app-animation-text 3s ease-in-out;
    animation-iteration-count: infinite;

    &:nth-child(1)  { animation-delay:  .1s *  1; opacity: calc(1 * 1)}
    &:nth-child(2)  { animation-delay:  .1s *  2; opacity: calc(1 * .9)}
    &:nth-child(3)  { animation-delay:  .1s *  3; opacity: calc(1 * .8)}
    &:nth-child(4)  { animation-delay:  .1s *  4; opacity: calc(1 * .7)}
    &:nth-child(5)  { animation-delay:  .1s *  5; opacity: calc(1 * .6)}
    &:nth-child(6)  { animation-delay:  .1s *  6; opacity: calc(1 * .5)}
    &:nth-child(7)  { animation-delay:  .1s *  7; opacity: calc(1 * .4)}
    &:nth-child(8)  { animation-delay:  .1s *  8; opacity: calc(1 * .3)}
    &:nth-child(9)  { animation-delay:  .1s *  9; opacity: calc(1 * .2)}
    &:nth-child(10) { animation-delay:  .1s * 10; opacity: calc(1 * .1)}
}


@keyframes app-animation-text {
    0% {
        font-variation-settings:'TRIP' 0;
        letter-spacing: 0em;
    }

    50% {
        font-variation-settings:'TRIP' 1;
        letter-spacing: -.02em;
    }

    100% {
        font-variation-settings:'TRIP' 0;
        letter-spacing: 0em;
    }
}
</style>
