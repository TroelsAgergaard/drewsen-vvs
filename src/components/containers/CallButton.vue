<template>
    <a class="header__call-button" href="tel:20468416"><i class="fas fa-phone"></i> 20 468 416</a>
</template>

<script>
export default {
    name: "CallButton"
}
</script>

<style scoped>
    .header__call-button {
        padding: 15px 25px;
        color: #fff;
        text-decoration: none;
        background-color: #502EFF;
        border-radius: 50px;
        z-index: 2;
    }

    .fas {
        margin: 0 5px 0 0;
    }
</style>