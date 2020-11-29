<template>
    <div class="projects-container">
        <md-list id="projects" class="md-double-line">
            <Project v-for="project in projects" :key="project.title"
                     :title="project.title"
                     :description="project.description"
                     :github-link="project.githubLink"
                     :language="project.language"
            />
        </md-list>
    </div>
</template>

<script>
    import Project from "./Project";

    export default {
        name: "Projects",
        components: {Project},
        data() {
            return {
                projects: []
            }
        },
        created: function () {
            fetch("/projects.json")
                .then(r => r.json())
                .then(data => {
                    this.projects = data.sort(function (a, b) {
                        return ('' + a.category).localeCompare(b.category);
                    });
                });
        }

    }
</script>

<style scoped>
    .projects-container {
        margin-left: 10%;
        margin-right: 10%;
        overflow: hidden;
    }

    #projects {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: space-between;
    }
</style>
