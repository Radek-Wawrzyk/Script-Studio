<template>
  <header class="header">
    <div class="container">
      <div class="header__content">
        <h1 class="header__title">
          Script Studio
        </h1>
        <p class="header__description">
          Awesome Software House
        </p>
        <div class="header__actions">
          <a class="button button--primary" href="#about" aria-title="Go about" title="Go About">
            Get Started
          </a>
        </div>
      </div>
    </div>
    <img class="header__background" alt="" src="~/assets/header.svg" />
  </header>
</template>

<script>

export default {
  name: 'home-header',
};

</script>

<style lang="scss" scoped src="./HomeHeader.scss" />
