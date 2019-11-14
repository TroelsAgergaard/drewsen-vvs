<template>
    <main class="main">
        <h1 class="main__header">Servies<br>& fabrikater</h1>
        <AppList></AppList>
        <AppGalleri></AppGalleri>
    </main>
</template>

<script>
    import AppList from '../ui/AppList'
    import AppGalleri from '../ui/AppGalleri'

    export default {
        name: "AppServices",
        components: {
            AppGalleri,
            AppList
        }
    }
</script>

<style scoped lang="scss" >
    .main {
        display: flex;
        flex-direction: column;
        box-sizing: border-box;
        background-image:url(../../assets/dots.jpg);
        background-repeat: repeat;
        height: 90vh;
        padding: 3.5rem 3.5rem;
    }
    .main__header {
        line-height: 2.8rem;
    }
</style>