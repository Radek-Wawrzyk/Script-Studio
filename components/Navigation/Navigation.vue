<template>
  <nav class="navigation" ref="navigation" :class="{'navigation--active' : scrollPosition > 140}">
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
    <ul
      class="navigation__menu"
      :class="{'navigation__menu--active': menuStatus}"
      :aria-expanded="menuStatus ? 'true' : 'false'"
    >
      <li class="navigation__menu-item">
        <a
          class="navigation__menu-link"
          href="#"
          title="Home"
          aria-label="Home"
          @click.prevent="handleClick('home')"
        >
          Home
        </a>
      </li>
      <li class="navigation__menu-item">
        <a
          class="navigation__menu-link"
          href="#"
          title="About"
          aria-label="About"
          @click.prevent="handleClick('about')"
        >
          About
        </a>
      </li>
      <!-- <li class="navigation__menu-item">
        <a class="navigation__menu-link" href="#works" title="Works" aria-label="Works">
          Works
        </a>
      </li> -->
      <li class="navigation__menu-item">
        <a
          class="navigation__menu-link"
          href="#" title="Service"
          aria-label="Service"
          @click.prevent="handleClick('services')"
         >
          Services
        </a>
      </li>
      <li class="navigation__menu-item">
        <a
          class="navigation__menu-link navigation__menu-link--primary"
          href="#contact"
          title="Contact"
          aria-label="Contact"
          @click.prevent="handleClick('contact')"
        >
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
    scrollPosition: null,
  }),
  methods: {
    toggleMenu() {
      this.menuStatus = !this.menuStatus;
    },
    handleScroll() {
      this.scrollPosition =  window.scrollY;
    },
    handleClick(parameter) {
      window.scrollTo({
        behavior: 'smooth',
        left: 0,
        top: document.querySelector(`#${parameter}`).offsetTop,
      });

      this.menuStatus === true ? this.menuStatus = false : false;
    },
  },
  mounted() {
    window.addEventListener("scroll", this.handleScroll);
  }
};

</script>

<style lang="scss" scoped src="./Navigation.scss" />
