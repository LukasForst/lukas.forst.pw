<template>
    <div>
        <img alt="My photo." src="../assets/me.png">

        <h2>Lukas Forst</h2>

        <md-button class="md-fab md-mini md-icon-button" :href="linkedin" target="_blank">
            <md-icon class="fa fa-linkedin"/>
        </md-button>

        <md-button class="md-fab md-mini md-icon-button" :href="github" target="_blank">
            <md-icon class="fa fa-github"/>
        </md-button>
    </div>
</template>

<script>
    export default {
        name: "About",
        data() {
            return {
                linkedin: 'https://www.linkedin.com/in/lukas-forst/',
                github: 'https://github.com/LukasForst'
            }
        }
    }
</script>

<style scoped>
    a {
        color: inherit;
    }
</style>