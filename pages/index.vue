<template>
  <main class="home">
    <navigation />
  </main>
</template>

<script>
import Navigation from '@/components/Navigation/Navigation.vue';

export default {
  name: 'home',
  components: {
    Navigation,
  },
};

</script>

<style lang="scss" scoped src="./index.scss" />
