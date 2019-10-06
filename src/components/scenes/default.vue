<template>
    <section class="scene-container">
        <header>
            <h1 class="scene-title">Mød<br>Medarbejderne</h1>
        </header>
        <Swiper></Swiper>
        <div class="flex-container">
            <h3>Kontakt os</h3>
            <CallButton class="test"></CallButton>
        </div>
    </section>
</template>

<script>
import Swiper from "../presentational/Swiper"
import CallButton from "../containers/CallButton"

export default {
    name: "Employees",
    components: {
        Swiper,
        CallButton
    }
}
</script>

<style scoped lang="scss">
    .scene-container {
        padding: 3.5rem 3.5rem;
        box-sizing: border-box;
        color: #502EFF;
    }
    .flex-container{
        display: flex;
        flex-direction: column;
        padding: 3.5rem 0 0 0;
        align-items: center;
    }
</style>