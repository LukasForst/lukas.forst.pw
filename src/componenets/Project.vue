<template>
    <div>
        <md-list-item class="project-link" :href="githubLink" target="_blank">

<!--            <md-avatar class="github-logo hover-logo">-->
<!--                <md-icon class="fa fa-github"/>-->
<!--            </md-avatar>-->

            <md-avatar class="hover-logo">
                <img class="language-icon" v-bind:src="languageIcon" alt="language icon"/>
            </md-avatar>

            <div class="md-list-item-text">
                <span class="md-title">{{title}}</span>
                <span>{{description}}</span>
            </div>
        </md-list-item>
    </div>
</template>

<script>
    export default {
        name: "Project",
        props: {
            title: String,
            description: String,
            githubLink: String,
            language: String
        },
        data() {
            return {
                languageIcon: require(`../assets/${this.language}.png`)
            }
        }
    }
</script>

<style scoped>
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