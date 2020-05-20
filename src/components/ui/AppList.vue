<template>
  <section>
    <ul class="services-list fa-ul">
      <li v-for="(service, id) in services" :key="id">
        <span class="fa-li"><i class="fas fa-tools"></i></span>{{ service }}
      </li>
    </ul>
    <!-- <ul v-if="$mq == 'sm'" class="services-list fa-ul">
      <li v-for="(fabrikater, id) in fabrikater" :key="id">
        <span class="fa-li"><i class="fas fa-cogs"></i></span>{{ fabrikater }}
      </li>
    </ul> -->
  </section>
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
      ],
      fabrikater: ["Vølund", "Viessmann", "Bosch", "Beretta"]
    };
  }
};
</script>

<style scoped lang="scss">
.services-list {
  list-style-type: none;
  line-height: calc(3rem + 1vw);
  font-size: calc(2rem + 1vw);
  margin: 0 3.5rem 0 3.5rem;
}
// .services-list:first-child {
//   margin-bottom: 3.5rem;
// }
.fas {
  color: rgb(232, 186, 51);
}

@media screen and (min-width: 768px) {
  .services-list {
    font-size: calc(1.5rem + 1vw);
    line-height: calc(2.5rem + 1vw);
    margin: 0 3.5rem 4.5rem 3.5rem;
  }
}
</style>
