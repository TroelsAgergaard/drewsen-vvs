<template>
  <header class="header">
    <div class="header__content-wrapper">
      <img class="header__logo" v-if="$mq === 'lg'" src="../../assets/drewsen-logo.png"
      alt="Drewsen VVS logo: Illustration
      af blå rørtang med påskriften Drewsen VVS" />
      <img class="header__logo" v-else src="../../assets/drewsen-logo-white.png"
      alt="Drewsen VVS logo: Illustration
      af blå rørtang med påskriften Drewsen VVS" />
      <img
        class="header__image"
        src="../../assets/bg.jpg"
        alt="Lukkeventil på vandrør"
      />
      <nav class="content-wrapper__nav">
        <ul class="nav__link-list">
          <li class="nav__link-list-item">
            <a class="link-list__anchor" href="#service">SERVICE</a>
          </li>
          <li class="nav__link-list-item">
            <a class="link-list__anchor" href="#service">FABRIKATER</a>
          </li>
          <li class="nav__link-list-item">
            <a class="link-list__anchor" href="#medarbejdere">MEDARBEJDERE</a>
          </li>
          <li class="nav__link-list-item">
            <a class="link-list__anchor" href="#historie">HISTORIE</a>
          </li>
          <li class="nav__link-list-item">
            <a class="link-list__anchor" href="#kontakt">KONTAKT</a>
          </li>
        </ul>
      </nav>
      <h1 class="header__title">
        Aut. VVS
        <br />Installatør i <br />Holbæk
      </h1>
      <CallButton class="content-wrapper__button"></CallButton>
    </div>
  </header>
</template>

<script>
import CallButton from "../ui/CallButton.vue";
export default {
  name: "AppHero",
  components: {
    CallButton
  }
};
</script>

<style scoped lang="scss">
.header__image {
  display: none;
}
.header__content-wrapper {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  height: 100%;
}
.content-wrapper__nav {
  display: none;
}
.header {
  --height: 65vh;
}
.header {
  height: var(--height);
  background: url(../../assets/bg.jpg);
  background-size: cover;
  padding: 3.5rem 3.5rem;
}
.header::after {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 75%;
  // background: linear-gradient(
  //   to bottom,
  //   rgb(232, 186, 51),
  //   rgba(rgb(232, 186, 51), 0)
  // );
}
.header__logo {
  width: 80%;
  z-index: 1;
}
.header__title {
  // color: #502eff;
  color: white;
  text-shadow: 1px 1px 35px #210000;
  font-size: 4rem;
  font-weight: bold;
  text-align: center;
  line-height: 4.5rem;
  z-index: 1;
}
.header__image {
  object-position: top;
}
@media screen and (min-width: 768px) {
  .header {
    padding: 0;
    background: none;
  }
  .header:after {
    display: none;
  }
  .header__content-wrapper {
    height: 100%;
    display: grid;
    grid-template-columns: 3.5rem 1fr 1fr 3.5rem;
    grid-template-rows: 3.5rem 1fr 3.5rem;
  }
  .header__logo {
    width: 200px;
    grid-column: 2;
    grid-row: 2;
    align-self: flex-start;
    justify-self: flex-start;
  }
  .header__title {
    color: #502eff;
    text-shadow: none;
    margin: 0;
    grid-column: 2;
    grid-row: 2;
    align-items: center;
    justify-self: center;
    font-size: 3.5rem;
    line-height: 3.3rem;
    transform: translateX(-1.75rem);
  }
  .content-wrapper__button {
    grid-column: 2;
    grid-row: 2;
    justify-self: center;
    align-self: end;
    transform: translateX(-1.75rem);
  }
  .header__image {
    display: block;
    width: 100%;
    min-height: 150%;
    max-height: 165%;
    box-shadow: 0 10px 40px -30px rgba(0, 0, 0, 1);
    grid-column: 3 / 5;
    grid-row: 1 / 3;
    object-fit: cover;
    object-position: bottom;
  }

  .content-wrapper__nav {
    display: block;
    grid-column: 3 / 4;
    grid-row: 2 / 2;
    align-self: start;
  }
  .nav__link-list {
    list-style: none;
    text-align: right;
    padding: 0;
    margin: 0;
  }
  .nav__link-list-item {
    margin-bottom: 1rem;
  }
  .link-list__anchor {
    text-decoration: none;
    color: white;
  }
}
</style>
