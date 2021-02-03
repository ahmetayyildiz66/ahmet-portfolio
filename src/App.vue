<template>
  <div class="app">
    <div class="container">
      <HeaderLayout />
      <router-view />
    </div>
  </div>
</template>
<script>
import HeaderLayout from "@/components/HeaderLayout.vue";

export default {
  name: "App",
  components: {
    HeaderLayout
  }
};
</script>
<style lang="scss">
@import "@/styles/scss/main.scss";

.app {
  background-color: $color-secondary;
  width: 100vw;
  height: 100vh;
}

.container {
  width: $size-container-width;
  margin: 0 auto;
  padding-top: 2rem;
  padding-bottom: 2rem;
}

a {
  text-decoration: none;

  &:hover,
  &:visited {
    color: inherit;
  }
}
</style>
