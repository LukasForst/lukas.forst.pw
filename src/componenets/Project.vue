<template>
    <div>
        <link rel="stylesheet"
              href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

        <md-list-item :href="githubLink" target="_blank">
            <md-avatar>
                <md-icon class="fa fa-github"/>
            </md-avatar>

            <div class="md-list-item-text">
                <span class="md-title">{{title}}</span>
                <span>{{description}}</span>
            </div>
        </md-list-item>
        <md-divider class="md-inset"></md-divider>
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

</style>