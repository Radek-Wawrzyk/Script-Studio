<template>
  <main class="home page">
    <navigation />
    <home-header />
  </main>
</template>

<script>
import Navigation from '@/components/Navigation/Navigation.vue';
import HomeHeader from '@/components/HomeHeader/HomeHeader.vue';

export default {
  name: 'home',
  components: {
    Navigation,
    HomeHeader,
  },
};

</script>

<style lang="scss" scoped src="./index.scss" />
