<template>
  <main class="home page">
    <navigation />
    <home-header />
    <home-about />
    <home-services />
  </main>
</template>

<script>
import Navigation from '@/components/Navigation/Navigation.vue';
import HomeHeader from '@/components/HomeHeader/HomeHeader.vue';
import HomeAbout from '@/components/HomeAbout/HomeAbout.vue';
import HomeServices from '@/components/HomeServices/HomeServices.vue';

export default {
  name: 'home',
  components: {
    Navigation,
    HomeHeader,
    HomeAbout,
    HomeServices,
  },
};

</script>

<style lang="scss" scoped src="./index.scss" />
