<template>
  <ul>
    <li>
      <p><i class="fas fa-user"></i><strong> {{ name }}</strong></p>
    </li>
    <li v-if="email">
      <a href="mailto:"><i class="fas fa-at"></i> {{ email }}</a>
    </li>
    <li>
      <a href="tel:"><i class="fas fa-phone-alt"></i> {{ tel }}</a>
    </li>
  </ul>
</template>

<script>
export default {
  name: "AppVcard",
  props: {
    name: String,
    email: String,
    tel: String
  }
};
</script>

<style scoped lang="scss">
ul {
  list-style: none;
  padding: 0 0 1rem 0;
}
ul:first-child{
    margin-top: 0;
}
li {
  margin: 0 0 5px 0;
  p,
  a {
    font-size: calc(1.2rem + 1vw);
    text-decoration: none;
    margin: 0;
  }
}
.vcards ul:last-of-type {
  padding: 0;
}

.fas {
  margin: 0 10px 0 0;
  color: rgb(232, 186, 51);
}
</style>
