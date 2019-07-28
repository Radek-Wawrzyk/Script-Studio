<template>
  <section class="sub-header">
    <img src="~/assets/bck.svg" alt="" class="sub-header__background"/>
    <div class="container">
      <h2 class="sub-header__title" data-aos="fade-up" data-aos-delay="100">
      {{ content }}
      </h2>
      <a class="button button--primary" @click.prevent="scrollTo(anchor)" :href="'#' + anchor" data-aos="fade-up" data-aos-delay="200">
        Go Services
      </a>
    </div>
  </section>
</template>

<script>
export default {
  name: 'sub-header',
  props: {
    content: {
      type: String,
      required: true,
    },
    anchor: {
      type: String,
      required: false,
    },
  },
   methods: {
    scrollTo(parameter) {
      window.scrollTo({
        behavior: 'smooth',
        left: 0,
        top: document.querySelector(`#${parameter}`).offsetTop,
      });
    },
  },
};

</script>

<style lang="scss" scoped src="./HomeSubHeader.scss" />
