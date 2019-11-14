<template>
    <ul class="services-list fa-ul">
        <li v-for="(service, id) in services" :key="id">
            <span class="fa-li"><i class="fas fa-tools"></i></span>{{ service }}
        </li>
    </ul>
</template>

<script>
    export default {
        name: "AppList",
        data: function() {
            return { 
                services: [
                    "VVS Arbejder",
                    "Blikkenslager",
                    "Gas service",
                    "Varmepumpe",
                    "Badeværelser",
                    "Jordvarme",
                    "Luft til vand"
                ]
            }
        }
    }
</script>

<style scoped lang="scss">
    .services-list {
        list-style-type: none;
        padding: 0;
    }
    .fa-ul {
        margin: 2.5rem;
        line-height: 2.5rem;
    }
    .fas {
        color: rgb(232, 186, 51);
    }
</style>