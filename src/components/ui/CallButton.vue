<template>
    <a class="call-button" href="tel:20468416"><i class="fas fa-phone-alt"></i> 20 468 416</a>
</template>

<script>
    export default {
        name: "CallButton"
    }
</script>

<style scoped>
    .call-button {
        padding: 15px 25px;
        width: fit-content;
        color: #fff;
        text-decoration: none;
        background-color: #502EFF;
        border-radius: 50px;
        font-size: calc(1.5rem + 1vw);
    }

    .fas {
        margin: 0 5px 0 0;
        color: rgb(232, 186, 51)
    }
</style>