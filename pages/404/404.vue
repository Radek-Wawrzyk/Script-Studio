<template>
  <main class="page error-page">
    <navigation />
    <section class="error">
      <img class="error__img" src="~/assets/404.svg" alt="" data-aos="fade-down" data-aos-delay="100"/>
      <div class="error__content" data-aos="fade-up" data-aos-delay="100">
        <p class="error__content-description">
          The page you are looking for does not exist... yet.
          PS. Do you need a page? We might be able to build one for you...
        </p>
        <nuxt-link to="/" class="button button--primary error__content-link" aria-label="Home" title="Home">
          Our portfolio
        </nuxt-link>
        <img class="error__content-img" src="~/assets/girl.svg" alt="" />
      </div>
    </section>
    <home-footer />
  </main>
</template>

<script>
import Navigation from '@/components/Navigation/Navigation.vue';
import HomeFooter from '@/components/HomeFooter/HomeFooter.vue';

export default {
  name: 'error',
  components: {
    Navigation,
    HomeFooter,
  },
};

</script>

<style lang="scss" scoped src="./404.scss" />
