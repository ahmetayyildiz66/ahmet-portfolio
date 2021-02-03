<template>
  <header class="header">
    <router-link to="/">
      <LogoIcon class="header__logo" />
    </router-link>
    <nav class="navigation">
      <router-link
        to="/projects"
        tag="a"
        class="navigation__item navigation__item--projects"
        >Projects</router-link
      >
      <router-link
        to="/"
        tag="a"
        class="navigation__item navigation__item--skills"
        >Skills</router-link
      >
    </nav>
  </header>
</template>

<script>
import LogoIcon from "../assets/LogoIcon.svg";

export default {
  name: "HeaderLayout",
  components: {
    LogoIcon
  }
};
</script>

<style lang="scss" scoped>
.header {
  color: $color-white;
  // background-color: orangered;
  height: $size-header-height;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
  font-size: 2rem;
}

.navigation {
  width: 27.5rem;
  height: 6.1rem;
  display: flex;
  align-items: center;
  justify-content: space-around;

  &__item {
    display: flex;
    align-items: center;
    text-align: center;
    padding: 0 1rem;
    border-bottom: 3px solid transparent;

    &:hover {
      border-bottom-color: $color-primary;
    }
  }
}
</style>
