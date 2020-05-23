<template>
  <main id="service" class="main">
    <h1 class="main__header">
      Services
      <br />
      & fabrikater
    </h1>
    <section class="flex-container">
      <AppList></AppList>
      <AppGalleri v-if="$mq === 'lg'"></AppGalleri>
    </section>
    <p>
    <strong class="mt10">Drewsens VVS er autoriseret VVS-installatør.</strong>
    <br><br>
    Det er vigtigt at vælge en autoriseret installatør af flere grunde. Først og fremmest er det en sikkerhed for at nye installationer eller andre arbejder udføreres korrekt. Med en <strong>autoriseret VVS-installatør</strong> undgås det således som altovervejende udgangspunkt at der opstår en situation, hvor arbejdet skal laves om, eller endnu værre end følgeskade som forsikringen ikke dækker, fordi arbejdet er udført af en uautoriseret VVS-installatør. 
    <br><br>
    Hos Drewsen VVS udfører vi alt inden for vores håndværksmæssige fagområde, det omfatter både <strong>blikkenslagerarbejde</strong>, <strong>gaskedelskift</strong>, og installation af <strong>alternative energikilder</strong> som <strong>jordvarme</strong> og <strong>luft-til-vand anlæg</strong>. Vi løser opgave for private kunder, erhvervs- og vi servicerer flere andelsboliger i København, og udfører renoveringsopgaver forskellige steder. Blandt andet på Dragsholm Slot.
    <br><br>
    Igennem årene har vi udført mange installationer og vi er eksperter på fabrikaterne – <strong>Viessmann</strong>, <strong>Beretta gaskedler</strong>, <strong>Bosch</strong> og <strong>Vølund varmeteknik</strong>. Du kan altid rådføre dig hos os, omkring alle VVS-relaterede opgaver, fabrikater eller indhente et uforpligtende tilbud. 
    </p>
  </main>
</template>

<script>
import AppList from "../ui/AppList";
import AppGalleri from "../ui/AppGalleri";

export default {
  name: "AppServices",
  components: {
    AppGalleri,
    AppList
  }
};
</script>

<style scoped lang="scss">
.main {
  display: flex;
  flex-direction: column;
  box-sizing: border-box;
  //   background-image: url(../../assets/dots.jpg);
  background-color: #2a28c7;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='863' height='103.6' viewBox='0 0 1000 120'%3E%3Cg fill='none' stroke='%232f2cdb' stroke-width='10.5' stroke-opacity='0.63'%3E%3Cpath d='M-500 75c0 0 125-30 250-30S0 75 0 75s125 30 250 30s250-30 250-30s125-30 250-30s250 30 250 30s125 30 250 30s250-30 250-30'/%3E%3Cpath d='M-500 45c0 0 125-30 250-30S0 45 0 45s125 30 250 30s250-30 250-30s125-30 250-30s250 30 250 30s125 30 250 30s250-30 250-30'/%3E%3Cpath d='M-500 105c0 0 125-30 250-30S0 105 0 105s125 30 250 30s250-30 250-30s125-30 250-30s250 30 250 30s125 30 250 30s250-30 250-30'/%3E%3Cpath d='M-500 15c0 0 125-30 250-30S0 15 0 15s125 30 250 30s250-30 250-30s125-30 250-30s250 30 250 30s125 30 250 30s250-30 250-30'/%3E%3Cpath d='M-500-15c0 0 125-30 250-30S0-15 0-15s125 30 250 30s250-30 250-30s125-30 250-30s250 30 250 30s125 30 250 30s250-30 250-30'/%3E%3Cpath d='M-500 135c0 0 125-30 250-30S0 135 0 135s125 30 250 30s250-30 250-30s125-30 250-30s250 30 250 30s125 30 250 30s250-30 250-30'/%3E%3C/g%3E%3C/svg%3E");
  background-repeat: repeat;
  padding: 3.5rem 3.5rem;
}
.flex-container {
  display: flex;
}
p {
  font-size: calc(1rem + 1vw);
  margin: 0;
}
.mt10{
  margin: 3.5rem 0 0 0;
}
// @media screen and (max-width: 768px) {
  // p {
  //   display: none;
  // }
// }
</style>
