<template>
    <md-list id="projects" class="md-double-line">
        <Project v-for="project in projects" :key="project.title"
                 :title="project.title"
                 :description="project.description"
                 :github-link="project.githubLink"
                 :language="project.language"
        />
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
                        title: 'Ktoolz',
                        description: 'Collection of extension functions for Kotlin.',
                        githubLink: 'https://github.com/blindspot-ai/ktoolz',
                        language: 'Kotlin'
                    },
                    {
                        title: 'Exposed Upsert',
                        description: 'PostgreSQL upsert implementation for Exposed framework .',
                        githubLink: 'https://github.com/LukasForst/exposed-upsert',
                        language: 'Kotlin'
                    },
                    {
                        title: 'Poll Bot',
                        description: 'Bot for Wire that can create polls.',
                        githubLink: 'https://github.com/wireapp/poll-bot',
                        language: 'Kotlin'
                    },
                    {
                        title: 'Charon',
                        description: 'Proxy mapping Slack API to Wire API.',
                        githubLink: 'https://github.com/wireapp/charon',
                        language: 'Python'
                    },
                    {
                        title: 'Pinder',
                        description: 'Website that chooses name of project for you.',
                        githubLink: 'https://github.com/LukasForst/pinder',
                        language: 'JavaScript'
                    },
                    {
                        title: 'Roman Echo Bot',
                        description: 'Simple echo bot for Wire using Roman proxy..',
                        githubLink: 'https://github.com/wireapp/echo-bot-roman',
                        language: 'Python'
                    },
                    {
                        title: 'Kotlin Gradle Template',
                        description: 'Template for publishing Gradle libraries to JCenter.',
                        githubLink: 'https://github.com/LukasForst/maven-library',
                        language: 'Kotlin'
                    },
                    {
                        title: '.NET Core Template',
                        description: 'Boilerplate for bigger projects using .NET Core 3.1.',
                        githubLink: 'https://github.com/LukasForst/dotnet-core-template',
                        language: 'C#'
                    },
                    {
                        title: 'Bachelor Thesis',
                        description: 'Scheduling optimization jobs on distributed platform.',
                        githubLink: 'https://github.com/LukasForst/bachelor-thesis',
                        language: 'Kotlin'
                    }
                ]
            }
        }
    }
</script>

<style scoped>
    #projects {
        text-align: center;
        width: 500px;
        max-width: 100%;
        display: inline-block;
        vertical-align: top;
        /*border: 1px solid rgba(#000, .12);*/
    }
</style>