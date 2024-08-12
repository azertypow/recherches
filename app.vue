<template>
    <div
        class="v-app"
    >
        <main>
            <NuxtPage/>
        </main>
    </div>
</template>

<style lang="scss" >
@font-face {
    font-family: 'oracle';
    src: url("@/assets/ABCOraclePlusVariable-Trial.ttf");
}

body {
    padding: 0;
    width: 100%;
    margin: 0;
    font-family: oracle, sans-serif;
    font-size: 10px;
}

.v-app {
    display: block;
    width: 100%;
}
</style>
