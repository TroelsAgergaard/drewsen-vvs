<template>
    <main class="main">
        <h1 class="main__header">Service<br>& fabrikater</h1>
        <ul class="services-list fa-ul">
            <li v-for="(service, id) in services" :key="id">
                <span class="fa-li"><i class="fas fa-tools"></i></span>{{ service }}
            </li>
        </ul>
        <Galleri></Galleri>
    </main>
</template>

<script>
import Galleri from '../containers/Galleri'
export default {
    name: "Main",
    components: {
        Galleri
    },
    data() {
        return { 
            services: [
                "VVS Arbejder",
                "Blikkenslager",
                "Gas service",
                "Varmepumpe",
                "Badeværelser",
                "Jordvarme"
            ]
        }
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
    .services-list {
        list-style-type: none;
        padding: 0;
    }
    .fa-ul {
        margin: 2.5rem;
        line-height: 2.5rem;
    }
</style>