<template>
    <section>
        <ul>
            <li><p><i class="fas fa-user"></i> {{ name }}</p></li>
            <li><a href="mailto:"><i class="fas fa-at"></i> {{ email }}</a></li>
            <li><a href="tel:"><i class="fas fa-phone-alt"></i> {{ tel }}</a></li>
        </ul>
    </section>
</template>

<script>
export default {
    name: "AppVcard",
    props: {
        name: String,
        email: String,
        tel: String
    }
}
</script>

<style scoped lang="scss">
    ul {
        list-style: none;
        padding: 0;
    }
    li {
        margin: 0 0 5px 0;
    }
    p {
        margin: 0;
    }
    a {
        text-decoration: none;
    }
    .fas{
        margin: 0 10px 0 0;
        color: rgb(232, 186, 51)
    } 
</style>