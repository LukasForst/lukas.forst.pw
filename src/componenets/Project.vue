<template>
  <div class="project">
    <md-list-item class="project-link" :href="githubLink" target="_blank">
      <md-avatar class="hover-logo">
        <img class="language-icon" :src="languageIcon" alt="language icon"/>
      </md-avatar>

      <div class="md-list-item-text">
        <span class="md-title">{{ title }}</span>
        <span class="description">{{ description }}</span>
      </div>
    </md-list-item>
  </div>
</template>

<script>
export default {
  name: 'Project',
  props: {
    title: String,
    description: String,
    githubLink: String,
    language: String
  },
  data() {
    return {
      languageIcon: require(`../assets/${this.language}.png`)
    };
  }
};
</script>

<style scoped>

.project {
  width: 500px;
}

@media screen and (max-width: 500px) {
  .description {
    visibility: hidden;
    display: none;
  }
}

.project-link {
  transition: background-color .5s;
}

.project-link:hover {
  background-color: whitesmoke;
}

.hover-logo {
  transition: transform .4s;
}

.project-link:hover .hover-logo {
  transform: scale(1.4);
}

.language-icon {
  height: 24px;
  width: 24px;
}
</style>