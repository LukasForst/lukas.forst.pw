<template>
  <div>
    <img class="photo-me" alt="My photo." src="../assets/me.png">

    <h1>Lukas Forst</h1>

    <div class="social-container">
      <!--   disable linked in button    -->
      <!--      <div class="social-button">-->
      <!--        <md-button class="md-fab md-mini md-icon-button" :href="linkedin" target="_blank">-->
      <!--          <md-icon class="fa fa-linkedin"/>-->
      <!--          <md-tooltip md-direction="bottom">-->
      <!--            <div class="tooltip-text">LinkedIn</div>-->
      <!--          </md-tooltip>-->
      <!--        </md-button>-->
      <!--      </div>-->

      <div class="social-button">
        <md-button class="md-fab md-mini md-icon-button" :href="cv" target="_blank">
          <md-icon class="fa fa-user"/>
          <md-tooltip md-direction="bottom">
            <div class="tooltip-text">CV</div>
          </md-tooltip>
        </md-button>
      </div>

      <div class="social-button">
        <md-button class="md-fab md-mini md-icon-button" :href="github" target="_blank">
          <md-icon class="fa fa-github"/>
          <md-tooltip md-direction="bottom">
            <div class="tooltip-text">Github</div>
          </md-tooltip>
        </md-button>
      </div>

      <div class="social-button">
        <md-button class="md-fab md-mini md-icon-button" :href="mail">
          <md-icon class="fa fa-envelope-o"/>
          <md-tooltip md-direction="bottom">
            <div class="tooltip-text">Mail</div>
          </md-tooltip>
        </md-button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Headline',
  data() {
    return {
      linkedin: 'https://www.linkedin.com/in/lukas-forst/',
      github: 'https://github.com/LukasForst',
      mail: 'mailto:lukas@forst.pw',
      cv: 'https://cv.forst.pw'
    };
  }
};
</script>

<style scoped>
a {
  color: inherit;
}

.photo-me {
  border-radius: 50%;
}

.social-container {
  display: flex;
  flex-flow: row;
  justify-content: center;
}

.social-container > .social-button ~ .social-button {
  padding-left: 5px;
}


.tooltip-text {
  font-size: 1rem;
}
</style>