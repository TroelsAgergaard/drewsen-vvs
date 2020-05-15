<template>
  <main id="service" class="main">
    <h1 class="main__header">
      Servies
      <br />
      & fabrikater
    </h1>
    <section class="flex-container">
      <AppList></AppList>
      <AppGalleri v-if="$mq === 'lg'"></AppGalleri>
    </section>
    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptas
      cupiditate quos ex perspiciatis vero! Architecto quo laboriosam distinctio
      fugiat error obcaecati culpa consectetur. Ipsam, odio error? Quas minima
      sunt iure animi nisi. Aut ut sit cupiditate ducimus neque hic, culpa
      repellendus velit fugiat vitae sint? Vero a quos blanditiis possimus?
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
  font-size: calc(0.8rem + 1vw);
  margin: 2.5rem 0 0 0;
}
@media screen and (max-width: 768px) {
  p {
    display: none;
  }
}
</style>
