<template>
  <main class="home page">
    <navigation />
    <home-header />
    <home-about />
    <home-sub-header
      anchor="services"
      content="The imaginative application of art and science to create a better future with you."
    />
    <home-services />
    <home-clients />
    <home-footer />
  </main>
</template>

<script>
import Navigation from '@/components/Navigation/Navigation.vue';
import HomeHeader from '@/components/HomeHeader/HomeHeader.vue';
import HomeAbout from '@/components/HomeAbout/HomeAbout.vue';
import HomeServices from '@/components/HomeServices/HomeServices.vue';
import HomeSubHeader from '@/components/HomeSubHeader/HomeSubHeader.vue';
import HomeClients from '@/components/HomeClients/HomeClients.vue';
import HomeFooter from '@/components/HomeFooter/HomeFooter.vue';

export default {
  name: 'home',
  components: {
    Navigation,
    HomeHeader,
    HomeAbout,
    HomeServices,
    HomeSubHeader,
    HomeClients,
    HomeFooter,
  },
};

</script>

<style lang="scss" scoped src="./index.scss" />
