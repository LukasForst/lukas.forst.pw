<template>
    <div>
        <md-list-item class="project-link" :href="githubLink" target="_blank">
            <md-avatar class="github-logo">
                <md-icon class="fa fa-github"/>
            </md-avatar>

            <div class="md-list-item-text">
                <span class="md-title">{{title}}</span>
                <span>{{description}}</span>
            </div>
        </md-list-item>
        <md-divider></md-divider>
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

    .github-logo {
        transition: transform .4s;
    }

    .project-link:hover .github-logo {
        transform: scale(1.4);
    }
</style>