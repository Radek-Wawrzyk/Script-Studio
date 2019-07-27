<template>
  <section class="about">
    <div class="container">
      <h2 class="about__header">
        Make digital
      </h2>
      <ul class="about__tiles">
        <li class="about__tile">
          <h3 class="about__tile-header">
            Technology
          </h3>
          <p class="about__tile-description">
            Technology for Marketing and Engagement, to develop integrated projects
            on digital touchpoints with the user.
          </p>
        </li>
        <li class="about__tile">
          <h3 class="about__tile-header">
            Marketing
          </h3>
          <p class="about__tile-description">
            We develop engagement strategies and manage content, user relationships,
            and media campaigns on digital platforms.
          </p>
        </li>
        <li class="about__tile about__tile--primary">
          <h3 class="about__tile-header">
            Insight
            <img src="~/assets/icons/data.svg" alt="" class="about__tile-icon"/>
          </h3>
          <p class="about__tile-description">
            We generate information through data: we analyze online interactions and
            develop useful reports for Marketing and Legal departments.
          </p>
        </li>
        <li class="about__tile">
          <h3 class="about__tile-header">
            INNOVATION
          </h3>
          <p class="about__tile-description">
            Lateral thinking and researching established and emerging technologies
            create the basis for cultivating innovation.
          </p>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>

export default {
  name: 'home-about',
};

</script>

<style lang="scss" scoped src="./HomeAbout.scss" />
