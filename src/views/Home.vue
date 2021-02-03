<template>
  <div class="home">
    <h1 class="fullname">
      <span class="fullname__item fullname__firstname">Ahmet</span>
      <span class="fullname__item fullname__lastname">AYYILDIZ</span>
    </h1>
    <h2 class="job">Front-End Developer</h2>
    <div class="social">
      <a href="https://github.com/ahmetayyildiz66">
        <GithubIcon />
      </a>
      <a href="https://www.linkedin.com/in/ahmet-ayyildiz-841452138/">
        <LinkedinIcon />
      </a>
      <a href="mailto:ahmetayyildiz66@gmail.com">
        <MailIcon />
      </a>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import GithubIcon from "@/assets/GithubIcon.svg";
import LinkedinIcon from "@/assets/LinkedinIcon.svg";
import MailIcon from "@/assets/MailIcon.svg";

export default {
  name: "Home",
  components: {
    GithubIcon,
    LinkedinIcon,
    MailIcon
  }
};
</script>

<style lang="scss" scoped>
.home {
  margin-top: 12rem;
  color: $color-white;
}

.fullname {
  &__item {
    font-weight: 500;
    font-size: 80px;
    display: block;
    letter-spacing: 2rem;
  }
}

.job {
  margin-top: 8.5rem;
  font-weight: 500;
  font-size: 3rem;
  color: $color-primary;
}

.social {
  margin-top: 3.5rem;
  width: 26.8rem;
  height: 7.2rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>
