<template>
  <section class="services" id="services">
    <img class="services__background" src="~/assets/steps.svg" alt="" />
    <div class="container">
      <div class="services__content">
        <header class="services__header">
          <h3 class="services__header-title">
            Customer journey
          </h3>
          <p class="services__header-description">
            We always follow professional Workflow and provide You
            best service with resealable costs.
          </p>
        </header>
        <ul class="services__list">
          <li class="services-tile" data-aos="fade-up" data-aos-delay="200">
            <span class="services-tile__icon">
              01
            </span>
            <div class="services-tile__content">
              <h4 class="services-tile__name">
                Getting to know your needs
              </h4>
              <p class="services-tile__description">
                We start our work by getting to know your vision of the finished product. We’ll do our best to understand your needs and provide you the best solutions possible.
              </p>
            </div>
          </li>
          <li class="services-tile" data-aos="fade-up" data-aos-delay="300">
            <span class="services-tile__icon">
              02
            </span>
            <div class="services-tile__content">
              <h4 class="services-tile__name">
                Full functional specification
              </h4>
              <p class="services-tile__description">
                We will summarize your needs and expectations so that you always have full control over the scope of work.
              </p>
            </div>
          </li>
          <li class="services-tile" data-aos="fade-up" data-aos-delay="400">
            <span class="services-tile__icon">
              03
            </span>
            <div class="services-tile__content">
              <h4 class="services-tile__name">
                Project Preview
              </h4>
              <p class="services-tile__description">
                We will send you a initial graphic design before signing the contract to make sure your requirements are met. 
              </p>
            </div>
          </li>
          <li class="services-tile" data-aos="fade-up" data-aos-delay="500">
            <span class="services-tile__icon">
              04
            </span>
            <div class="services-tile__content">
              <h4 class="services-tile__name">
                Signing a contract
              </h4>
              <p class="services-tile__description">
                When we will gather enough data to assure your satisfaction, We will sign the contract on terms as convenient as possible for you.
              </p>
            </div>
          </li>
          <li class="services-tile" data-aos="fade-up" data-aos-delay="600">
            <span class="services-tile__icon">
              05
            </span>
            <div class="services-tile__content">
              <h4 class="services-tile__name">
                Demo access
              </h4>
              <p class="services-tile__description">
                We will give you access to the test version of your product so that you can personally ensure that it meets your expectations. We’ll use your feedback to make even better product. 

              </p>
            </div>
          </li>
          <li class="services-tile" data-aos="fade-up" data-aos-delay="700">
            <span class="services-tile__icon">
              06
            </span>
            <div class="services-tile__content">
              <h4 class="services-tile__name">
                Release
              </h4>
              <p class="services-tile__description">
                We will guide you through the process of starting up your website, and provide you with documentation that will make editing the website a piece of cake - for everyone, even without technical background.

              </p>
            </div>
          </li>
          <li class="services-tile" data-aos="fade-up" data-aos-delay="800">
            <span class="services-tile__icon">
              07
            </span>
            <div class="services-tile__content">
              <h4 class="services-tile__name">
                Post-release support
              </h4>
              <p class="services-tile__description">
                We provide technical support to our products for as long, as you wish. 
              </p>
            </div>
          </li>
          
        </ul>
      </div>
    </div>
  </section>
</template>

<script>

export default {
  name: 'home-services',
};

</script>

<style lang="scss" scoped src="./HomeServices.scss" />
