<template>
  <address id="kontakt" class="vcard">
    <h1 class="vcard__header">Kontakt<br />& information</h1>
    <section class="flex-wrapper">
      <section class="vcards">
        <AppVcard
          name="Torben Drewsen"
          email="torben@drewsen-vvs.dk"
          tel="20 46 84 16"
        ></AppVcard>
        <AppVcard
          name="Bo Larsen"
          email="bo@drewsen-vvs.dk"
          tel="40 26 62 30"
        ></AppVcard>
        <AppVcard name="LYGAS" tel="50 13 14 15"></AppVcard>
      </section>
      <section class="adresse">
        <h2>Adresser</h2>
        <p>Kontor, Lærkevej 16.</p>
        <p></p>
        <p>Værksted, Rebslagervej 6D.</p>
        <p>4300 Holbæk</p>
        <img class="header__logo" src="../../assets/drewsen-logo.png" alt="">
      </section>
    </section>
  </address>
</template>

<script>
import AppVcard from "../ui/AppVcard";
export default {
  name: "kontakt",
  components: {
    AppVcard
  }
};
</script>

<style scoped lang="scss">
.header__logo {
display: none;
}
.flex-wrapper {
  display: block;
}
.vcard {
  background-color: #ffffff;
  // background: linear-gradient(
  //     to top,
  //     rgb(232, 186, 51),
  //     rgba(rgb(232, 186, 51), 0) 60%
  // );
  color: #502eff;
  padding: 3.5rem 3.5rem;
  font-style: normal;
  z-index: 2;
}
.vcard__header {
  line-height: 2.8rem;
}
.adresse {
  margin: 3.5rem 0 0 0;
  color: #502eff;
}
p {
  margin: 1vw 0;
  font-size: calc(1.4rem + 1vw);
}
h2 {
  font-size: calc(1.5rem + 1vw);
  margin: 0;
}
@media screen and (min-width: 768px) {
.header__logo {
    display: block;
    margin: 3.5rem 0 0 0;
    width: 30vw;
}
  .flex-wrapper {
    display: flex;
    justify-content: space-between;
  }
  .adresse {
    margin: 0;
  }
}
//add media query to fix h2 margin top on large devices
</style>
