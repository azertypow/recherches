<template>
    <section
        class="v-animation"
    >
        <div class="text-container">
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

.text-container {
    position: fixed;
    top: calc(50% - 1.55rem);
    left: 50%;
    transform: translate(-50%, -50%);
    width: 100%;
}

.text {
    line-height: .75em;
    animation: app-animation-text 3s ease-in-out;
    animation-iteration-count: infinite;

    &:nth-child(1)  { animation-delay:  .25s *  1; }
    &:nth-child(2)  { animation-delay:  .25s *  2; }
    &:nth-child(3)  { animation-delay:  .25s *  3; }
    &:nth-child(4)  { animation-delay:  .25s *  4; }
    &:nth-child(5)  { animation-delay:  .25s *  5; }
    &:nth-child(6)  { animation-delay:  .25s *  6; }
    &:nth-child(7)  { animation-delay:  .25s *  7; }
    &:nth-child(8)  { animation-delay:  .25s *  8; }
    &:nth-child(9)  { animation-delay:  .25s *  9; }
    &:nth-child(10) { animation-delay:  .25s * 10; }
    &:nth-child(11) { animation-delay:  .25s * 11; }
    &:nth-child(12) { animation-delay:  .25s * 12; }
    &:nth-child(13) { animation-delay:  .25s * 13; }
    &:nth-child(14) { animation-delay:  .25s * 14; }
    &:nth-child(15) { animation-delay:  .25s * 15; }
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
