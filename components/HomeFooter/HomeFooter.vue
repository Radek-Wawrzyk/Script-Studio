<template>
  <footer class="footer">
    <div class="container">
      <img class="footer__logo" src="~/assets/logo.svg" alt="" />
      <p class="footer__description">
        The full-stack design team who focuses on digital products whatever they are.
      </p>
      <ul class="footer__socials">
        <li class="footer__social">
          <a href="#" class="footer__social-link" title="Script-Studio Facebook" aria-label="Script-Studio Facebook">
            <img src="~/assets/icons/Facebook.svg" alt="" class="footer__social-icon" />
          </a>
        </li>
        <li class="footer__social">
          <a href="#" class="footer__social-link" title="Script-Studio Twitter" aria-label="Script-Studio Twitter">
            <img src="~/assets/icons/Twitter.svg" alt="" class="footer__social-icon" />
          </a>
        </li>
        <li class="footer__social">
          <a href="#" class="footer__social-link" title="Script-Studio Google+" aria-label="Script-Studio Google+">
            <img src="~/assets/icons/Google+.svg" alt="" class="footer__social-icon" />
          </a>
        </li>
      </ul>
      <p class="footer__copyright">
        © 2019 all rights reserved
      </p>
    </div>
  </footer>
</template>

<script>

export default {
  name: 'footer',
};

</script>

<style lang="scss" scoped src="./HomeFooter.scss" />
