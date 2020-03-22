<template>
    <div>
        <link rel="stylesheet"
              href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

        <md-list-item :href="githubLink" target="_blank">
            <md-avatar>
                <md-icon class="fa fa-github"/>
            </md-avatar>
            <span class="md-list-item-text">
                {{title}}
            </span>
            <span class="md-list-item-text">
                {{description}}
            </span>
        </md-list-item>
    </div>
</template>

<script>
    export default {
        name: "Project",
        props: {
            title: String,
            description: String,
            githubLink: String
        }
    }
</script>

<style scoped>

</style>