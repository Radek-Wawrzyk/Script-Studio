<template>
  <header class="header">
    <div class="header__content">
      <h1 class="header__title">
        Script Studio
      </h1>
      <p class="header__description">
        Awesome Software House
      </p>
      <div class="header__actions">
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
