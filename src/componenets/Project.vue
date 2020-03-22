<template>
    <div>
        <md-list-item :href="githubLink" target="_blank">
            <md-avatar>
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
    a {
        color: inherit;
    }
</style>