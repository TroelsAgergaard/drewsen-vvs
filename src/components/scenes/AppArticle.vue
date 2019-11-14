<template>
    <article class="article">
        <h1 class="article__heading">Vores<br>historie</h1>
        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Distinctio ipsum aperiam animi et quis deserunt deleniti libero, repellat dicta voluptas fugiat dolorem asperiores dolor doloribus similique suscipit aut incidunt facilis accusamus natus culpa repudiandae ad ducimus velit? Veritatis, aut. Ea sapiente est similique vel a impedit repellendus! Nisi, ratione nulla?</p>
    </article>
</template>

<script>
    export default {
        name: "AppAtricle"
    }
</script>

<style scoped lang="scss">
    .article{
        background-image:url(../../assets/dots.jpg);
        background-repeat: repeat;
        height: 90vh;
        padding: 3.5rem 3.5rem;
        box-sizing: border-box;
    }
    .article__heading{
        font-size: 2em;
        line-height: 2.8rem;
    }
</style>