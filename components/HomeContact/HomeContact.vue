<template>
  <section class="contact" id="contact">
    <img src="~/assets/contact.svg" alt="" class="contact__background" />
    <div class="container">
      <div class="contact__content">
        <header class="contact__header">
          <h3 class="contact__header-title">
            Drop Us a line
          </h3>
          <p class="contact__header-description">
            We can't wait to work with You on something cool!
          </p>
        </header>
        <form class="contact__form" @submit.prevent="submitForm" data-aos="fade-up" data-aos-delay="100">
          <div class="form__group">
            <input
              class="form__input"
              name="fullname"
              placeholder="Fullname"
              v-validate="'required'"
              v-model="fullname"
            />
            <transition name="fade-form">
              <span class="form__error" v-if="errors.has('fullname')">
                {{errors.first('fullname')}}
              </span>
            </transition>
          </div>
          <div class="form__group">
            <input
              class="form__input"
              name="email"
              placeholder="Email"
              v-validate="'required|email'"
              v-model="email"
            />
            <transition name="fade-form">
              <span class="form__error" v-if="errors.has('email')">
                {{errors.first('email')}}
              </span>
            </transition>
          </div>
          <div class="form__group">
            <input
              class="form__input"
              name="phone"
              placeholder="Phone number"
              v-model="phone"
            />
          </div>
          <div class="form__group">
            <textarea
              class="form__textarea"
              name="message"
              v-validate="'required'"
              v-model="message"
              rows="7"
              autocorrect="off"
              autocapitalize="off"
              spellcheck="false"
              placeholder="Message"
            >
            </textarea>
            <transition name="fade-form">
              <span class="form__error" v-if="errors.has('message')" >
                {{errors.first('message')}}
              </span>
            </transition>
          </div>
          <div class="form__group">
            <input class="form__checkbox" id="styled-checkbox-2" name="privacy" v-validate="'required'" type="checkbox" v-model="privacyData" />
            <label class="form__checkbox-label" for="styled-checkbox-2">
              I have accepted the
              <a href="#" class="form__link" aria-label="Term and Conditions" title="Term and Conditions">
                Term and Conditions
              </a>
            </label>
            <transition name="fade-form">
              <span class="form__error" v-if="errors.has('privacy')" >
                {{errors.first('privacy')}}
              </span>
            </transition>
          </div>
          <div class="form__group">
            <button class="button button--primary contact__button">
              Send a message
            </button>
          </div>
          <transition name="fade-form">
            <div class="form__group" v-if="status === 'success'">
              <span class="form__notification form__notification--success">You have sent a message! We will respond you as fast as we can!</span>
            </div>
            <div class="form__group" v-if="status === 'error'">
              <span class="form__notification form__notification--error">You haven't sent a message! There is a problem with our server</span>
            </div>
          </transition>
        </form>
      </div>
    </div>
  </section>
</template>

<script>
import axios from "axios";

export default {
  name: 'home-contact',
  data: () => ({
    fullname: '',
    email: '',
    message: '',
    phone: '',
    privacyData: false,
    status: null,
  }),
  methods: {
    async submitForm() {
      const valid = await this.$validator.validateAll();
      valid ? this.sendRequest() : false;
    },
    async sendRequest() {
      try {
        const response = await axios.post('sendMail.php', {
          fullName: this.fullname,
          email: this.email,
          message: this.message,
          phone: this.phone,
        });

        console.log(this.response);
        this.status = 'success';
      } catch (err) {
        console.log(err);
        this.status = 'error';
      }
    },
  },
};

</script>

<style lang="scss" scoped src="./HomeContact.scss" />
