<template>
  <div>
    <transition name="fade-page" mode="out-in">
      <nuxt />
    </transition>
  </div>
</template>

<script>
import AOS from 'aos';

export default {
  name: 'app-layout',
  created() {
    if (process) {
      if (process.browser) {
        AOS.init({
           once: true,
           duration: 1000,
        });
      }
    }
  },
};

</script>
