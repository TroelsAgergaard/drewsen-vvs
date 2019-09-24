<template>
    <header class="header">
        <img class="header__logo" src="../../assets/drewsen-logo.png" alt="Drewsen VVS logo: Illustration af blå rørtang med påskriften Drewsen VVS">
        <h1 class="header__title">Aut. VVS Installatør</h1>
        <call-button></call-button>
    </header>
</template>

<script>
import CallButton from "../containers/CallButton.vue"
export default {
    name: "Hero",
    components: {
        CallButton
    }
}
</script>

<style scoped lang="scss">
    .header {
        --height: 70vh;
    }
    .header {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        height: var(--height);
        background: url(../../assets/bg.jpg);
        background-size: cover;
        z-index: 0;
    }
    .header:after{
        content: '';
        position: absolute;
        left: 0;
        top: 0;
        width: 100%;
        height: var(--height);
        // background-color: rgba(211,411,211,0.3);
        background: linear-gradient(
            to bottom,
            rgb(232, 186, 51),
            rgba(rgb(232, 186, 51), 0)
        );
        z-index: 1;
    }
    .header__logo {
        width: 55vw;
        margin: 15px 0;
        z-index: 2;
        align-self: center;
        justify-self: flex-start;
    }
    .header__title {
        color: #502EFF;
        font-size: 4rem;
        font-weight: bold;
        text-align: center;
        line-height: 4rem;
        z-index: 2;
    }
</style>