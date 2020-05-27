<template>
  <section id="medarbejdere" class="scene-container">
    <header>
      <h1 class="heading">
        De
        <br />ansatte
      </h1>
    </header>
    <AppSwiper v-if="$mq === 'sm'"></AppSwiper>
    <section class="employe-list" v-if="$mq === 'lg'">
      <figure>
        <img src="../../assets/torben.png" alt />
        <h2 class="employe-title">Torben Drewsen</h2>
        <h3 class="employe-subtitle">Indehaver</h3>
      </figure>
      <figure>
        <img src="../../assets/bo.png" alt />
        <h2 class="employe-title">Bo Larsen</h2>
        <h3 class="employe-subtitle">Indehaver</h3>
      </figure>
      <figure>
        <img src="../../assets/alexander.png" alt />
        <h2 class="employe-title">Alexander Heincihson</h2>
        <h3 class="employe-subtitle">Svend</h3>
      </figure>
      <figure>
        <img src="../../assets/bodil.png" alt />
        <h2 class="employe-title">Bodil Drewsen</h2>
        <h3 class="employe-subtitle">Kontor</h3>
      </figure>
    </section>
    <div class="flex-container">
      <p>Kontakt os</p>
      <CallButton class="test"></CallButton>
    </div>
  </section>
</template>

<script>
import AppSwiper from "../ui/AppSwiper";
import CallButton from "../ui/CallButton";

export default {
  name: "Employees",
  components: {
    AppSwiper,
    CallButton
  }
};
</script>

<style scoped lang="scss">
figure {
  margin: 3.5rem 0 1.5rem 0;
}
.employe-title {
  text-align: center;
  font-size: calc(0.5rem + 1vw);
  font-weight: lighter;
  margin: 1rem 0 0 0;
}
.employe-subtitle {
  color: #bebebe;
  text-align: center;
  font-weight: lighter;
  font-size: calc(0.5rem + 1vw);
  margin: 0.2rem 0 1rem 0;
  color: rgb(232, 186, 51);
}
.employe-list {
  display: flex;
  justify-content: space-between;
}
.employe-list img {
  width: 20vw;
}
.scene-container {
  padding: 3.5rem 3.5rem;
  box-sizing: border-box;
  color: #502eff;
}
.flex-container {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.heading {
  line-height: 2rem;
  font-size: 2em;
  margin: 0 !important;
}
</style>
