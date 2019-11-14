<template>
    <section class="scene-container">
        <header>
            <h1 class="heading">De<br>ansatte</h1>
        </header>
        <AppSwiper></AppSwiper>
        <div class="flex-container">
            <h3>Kontakt os</h3>
            <CallButton class="test"></CallButton>
        </div>
    </section>
</template>

<script>
    import AppSwiper from "../ui/AppSwiper"
    import CallButton from "../ui/CallButton"

    export default {
        name: "Employees",
        components: {
            AppSwiper,
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
    .heading{
        line-height: 2rem;
        font-size: 2em;
    }
</style>
