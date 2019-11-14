<template>
    <address class="vcard">
        <h1 class="vcard__header">Kontakt<br>& information</h1>
        <AppVcard name="Torben Drewsen" email="torben@drewsen-vvs.dk" tel="20 46 84 16"></AppVcard>
        <AppVcard name="Bo Larsen" email="bo@drewsen-vvs.dk" tel="40 26 62 30"></AppVcard>
        <AppVcard name="LYGAS" tel="50 13 14 15"></AppVcard>
        <section class="adresse">
            <b>Adresse:</b>
            Lærkevej 16, 4300 Holbæk
        </section>
        <section>
            <b>Værksted:</b>
            Rebslagervej 6D, 4300 Holbæk
        </section>
    </address>
</template>

<script>
    import AppVcard from '../ui/AppVcard'
    export default {
        name: "kontakt",
        components: {
            AppVcard
        }
    }
</script>

<style scoped lang="scss">
    .vcard{
        background: #fff;
        color: #502EFF;
        padding: 3.5rem 3.5rem;
        font-style: normal;
    }
    .vcard__header{
        line-height: 2.8rem;
    }
    .adresse{
        margin: 0 0 0.5rem 0;
    }
</style>