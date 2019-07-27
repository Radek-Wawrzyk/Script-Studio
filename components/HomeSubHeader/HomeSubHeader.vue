<template>
  <section class="sub-header">
    <img src="~/assets/bck.svg" alt="" class="sub-header__background" />
    <div class="container">
      <h2 class="sub-header__title">
      {{ content }}
      </h2>
      <a class="button button--primary" :href="'#' + anchor">
        Get started
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
};

</script>

<style lang="scss" scoped src="./HomeSubHeader.scss" />
