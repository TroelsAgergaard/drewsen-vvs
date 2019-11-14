<template>
    <header class="header">
        <div class="header-content-wrapper">
            <img class="header__logo" src="../../assets/drewsen-logo.png" alt="Drewsen VVS logo: Illustration af blå rørtang med påskriften Drewsen VVS">
            <h1 class="header__title">Aut. VVS<br>Installatør</h1>
            <call-button></call-button>
        </div>
    </header>
</template>

<script>
import CallButton from "../ui/CallButton.vue"
export default {
    name: "AppHero",
    components: {
        CallButton
    }
}
</script>

<style scoped lang="scss">
    .header-content-wrapper {
        text-align: center;
        z-index: 2;
    }
    .header {
        --height: 70vh;
    }
    .header {
        display: flex;
        flex-direction: column;
        justify-content: center;
        height: var(--height);
        background: url(../../assets/bg.jpg);
        background-size: cover;
    }
    .header:after{
        content: '';
        position: absolute;
        left: 0;
        top: 0;
        width: 100%;
        height: var(--height);
        background: linear-gradient(
            to bottom,
            rgb(232, 186, 51),
            rgba(rgb(232, 186, 51), 0)
        );
        z-index: 1;
    }
    .header__logo {
        width: 55vw;
        align-self: center;
        justify-self: flex-start;
    }
    .header__title {
        color: #502EFF;
        font-size: 4rem;
        margin: 5rem 0 3.5rem 0;
        font-weight: bold;
        text-align: center;
        line-height: 4rem;
    }
</style>