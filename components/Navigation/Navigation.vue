<template>
  <nav class="navigation" ref="navigation">
    <figure class="navigation__logo">
      <a href="#" title="home" aria-label="home">
        <img class="navigation__logo-img" alt="SpaceJobs" src="~/assets/logo.svg" />
      </a>
    </figure>
    <button
      class="navigation__button"
      :class="{'navigation__button--active': menuStatus}"
      :aria-expanded="menuStatus ? 'true' : 'false'"
      @click="toggleMenu"
      aria-label="Open menu"
    >
      <span class="navigation__button-bar"></span>
      <span class="navigation__button-bar"></span>
      <span class="navigation__button-bar"></span>
    </button>
    <ul class="navigation__menu" :class="{'navigation__menu--active': menuStatus}">
      <li class="navigation__menu-item">
        <a class="navigation__menu-link" href="#" title="Home" aria-label="Home">
          Home
        </a>
      </li>
      <li class="navigation__menu-item">
        <a class="navigation__menu-link" href="#about" title="About" aria-label="About">
          About
        </a>
      </li>
      <!-- <li class="navigation__menu-item">
        <a class="navigation__menu-link" href="#works" title="Works" aria-label="Works">
          Works
        </a>
      </li> -->
      <li class="navigation__menu-item">
        <a class="navigation__menu-link" href="#services" title="Service" aria-label="Service">
          Services
        </a>
      </li>
      <li class="navigation__menu-item">
        <a class="navigation__menu-link navigation__menu-link--primary" href="#contact" title="Contact" aria-label="Contact">
          Contact Us
        </a>
      </li>
    </ul>
  </nav>
</template>

<script>

export default {
  name: 'navigation',
  data: () => ({
    menuStatus: false,
  }),
  methods: {
    toggleMenu() {
      this.menuStatus = !this.menuStatus;
    },
  },
};

</script>

<style lang="scss" scoped src="./Navigation.scss" />
