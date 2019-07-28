<template>
  <div>
    <nuxt />
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
        });
      }
    }
  },
};

</script>
