<template>
    <div>
        <img class="photo-me" alt="My photo." src="../assets/me.png">

        <h1>Lukas Forst</h1>

        <md-button class="md-fab md-mini md-icon-button" :href="github" target="_blank">
            <md-icon class="fa fa-github"/>
        </md-button>

        <md-button class="md-fab md-mini md-icon-button" :href="linkedin" target="_blank">
            <md-icon class="fa fa-linkedin"/>
        </md-button>

        <md-button class="md-fab md-mini md-icon-button" :href="mail">
            <md-icon class="fa fa-envelope-o"/>
        </md-button>
    </div>
</template>

<script>
    export default {
        name: "About",
        data() {
            return {
                linkedin: 'https://www.linkedin.com/in/lukas-forst/',
                github: 'https://github.com/LukasForst',
                mail: 'mailto:lukas@forst.pw'
            }
        }
    }
</script>

<style scoped>
    a {
        color: inherit;
    }

    .photo-me {
        border-radius: 50%;
    }
</style>