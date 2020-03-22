<template>
    <md-list id="projects" class="md-double-line">
        <Project v-for="project in projects" :title="project.title" :key="project.title"
                 :description="project.description" :github-link="project.githubLink"/>
    </md-list>
</template>

<script>
    import Project from "./Project";

    export default {
        name: "Projects",
        components: {Project},
        data() {
            return {
                projects: [
                    {
                        title: 'Pinder',
                        description: 'Simple Vue website which chooses name of the project for you.',
                        githubLink: 'https://github.com/LukasForst/pinder'
                    }
                ]
            }
        }
    }
</script>

<style scoped>
    #projects {
        text-align: center;
        width: 320px;
        max-width: 100%;
        display: inline-block;
        vertical-align: top;
        /*border: 1px solid rgba(#000, .12);*/
    }
</style>