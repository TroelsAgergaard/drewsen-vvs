<template>
    <div class="flex-wrapper">
        <section class="galleri-grid">
            <img class="galleri-img beretta" src="../../assets/beretta.jpg" alt="">
            <img class="galleri-img bosch" src="../../assets/bosch.jpg" alt="">
            <img class="galleri-img viessmann" src="../../assets/viessmann.jpg" alt="">
            <img class="galleri-img voelund" src="../../assets/voelund.jpg" alt="">
        </section>
    </div>
</template>

<script>
    export default {
        name: "Galleri"
    }
</script>

<style scoped lang="scss">
    .flex-wrapper { /* Galleri fill remaning space */
        flex-grow: 1;
        flex-shrink: 1;
        flex-basis: auto;
    }
    .galleri-grid {
        height: 100%;
        display: grid;
        grid-gap: 1vh;
        grid-template-columns: repeat(3, 1fr);
        grid-template-rows: 1fr 1.2fr;
    }
    .galleri-img {
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
    .beretta {
        grid-column: 1 / 2;
        grid-row: 1 / 3;
        object-position: top;
    }
    .viessmann {
        grid-column: 2 / 4;
        grid-row: 1 / 2;
    }
    .bosch {
        grid-column: 2 / 2;
        grid-row: 2 / 3;
        object-position: 85%;
    }
    .vuelund {
        grid-column: 3 / 4;
        grid-row: 2 / 3;
    }
</style>