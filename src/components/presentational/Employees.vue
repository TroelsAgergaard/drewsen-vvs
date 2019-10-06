<template>
    <section class="swiper-container">
        <article class="swiper-wrapper">
            <div class="swiper-slide">
                <img src="../../assets/torben.png" alt="">
                <h1 class="employe-title">Torben Drewsen</h1>
                <h2 class="employe-subtitle">Indehaver</h2>
            </div>
            <div class="swiper-slide">
                <img src="../../assets/bo.png" alt="">
                <h1 class="employe-title">Bo Larsen</h1>
                <h2 class="employe-subtitle">Indehaver</h2>
            </div>
            <div class="swiper-slide">
                <img src="../../assets/alexander.png" alt="">
                <h1 class="employe-title">Alexander</h1>
                <h2 class="employe-subtitle">Lærling</h2>
            </div>
            <div class="swiper-slide">
                <img src="../../assets/bodil.png" alt="">
                <h1 class="employe-title">Bodil Drewsen</h1>
                <h2 class="employe-subtitle">Kontor</h2>
            </div>
        </article>
        <div class="swiper-button-prev"></div>
        <div class="swiper-button-next"></div>
    </section>
</template>

<script>
import Swiper from 'swiper'

export default {
    name: "Employees",
        mounted: function() {
            var mySwiper = new Swiper('.swiper-container', {
                // Optional parameters
                direction: "horizontal",
                loop: true,
                spaceBetween: 50,
                effect: "slide"
                // Navigation arrows
                // navigation: {
                // nextEl: ".swiper-button-next",
                // prevEl: ".swiper-button-prev",
                // }
            })
        }

}
</script>

<style scoped lang="scss">
    .swiper-container {
        box-sizing: border-box;
        width: 100%;
        height: 90vh;
        padding: 3.5rem 3.5rem;
    }
    .swiper-slide{
        width: 100%;
        display: flex;
        align-items: center;
        flex-direction: column;
    }
    .swiper-slide img {
        width: 60vw;
        box-shadow: 0 0 25px rgba(0, 0, 0, 0.3);
    }
    .employe-title {
        color: #502EFF;
        font-weight: lighter;
        font-size: 1.5rem;
        margin: 2.5rem 0 0 0;
    }
    .employe-subtitle{
        color: #BEBEBE;
        font-weight: lighter;
        font-size: 1.2rem;
        margin: 0.5rem 0 0 0;
    }
    .swiper-button-prev, .swiper-button-next {
        top: 35%;
    }
</style>