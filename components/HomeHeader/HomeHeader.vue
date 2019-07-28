<template>
  <header class="header" id="home">
    <div class="header__content">
      <h1 class="header__title" data-aos="fade-right" data-aos-delay="200">
        Script Studio
      </h1>
      <p class="header__description" data-aos="fade-right" data-aos-delay="300">
        Awesome Software House
      </p>
      <div class="header__actions" data-aos="fade-right" data-aos-delay="400">
        <a class="button button--primary" href="#about" aria-title="Go about" title="Go About">
          Get started
        </a>
        <!-- <a class="header__link" href="#portfolio" aria-title="Go about" title="Go About">
          Portfolio
        </a> -->
      </div>
    </div>
    <img class="header__background" alt="" src="~/assets/header.svg" />
    <div class="header__actions header__actions--mobile">
      <a class="button button--primary" href="#portfolio" aria-title="Go about" title="Go About">
        Portfolio
      </a>
    </div>
  </header>
</template>

<script>

export default {
  name: 'home-header',
};

</script>

<style lang="scss" scoped src="./HomeHeader.scss" />
