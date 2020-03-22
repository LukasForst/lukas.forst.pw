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
                        language: 'kotlin'
                    },
                    {
                        title: 'Exposed Upsert',
                        description: 'PostgreSQL upsert implementation for Exposed framework.',
                        githubLink: 'https://github.com/LukasForst/exposed-upsert',
                        language: 'kotlin'
                    },
                    {
                        title: 'Charon',
                        description: 'Proxy mapping Slack API to Wire API.',
                        githubLink: 'https://github.com/wireapp/charon',
                        language: 'python'
                    },
                    {
                        title: 'Poll Bot',
                        description: 'Bot for Wire that can create polls.',
                        githubLink: 'https://github.com/wireapp/poll-bot',
                        language: 'kotlin'
                    },
                    {
                        title: 'Pinder',
                        description: 'Website that chooses name of project for you.',
                        githubLink: 'https://github.com/LukasForst/pinder',
                        language: 'vuejs'
                    },
                    {
                        title: 'Roman Echo Bot',
                        description: 'Simple echo bot for Wire using Roman proxy.',
                        githubLink: 'https://github.com/wireapp/echo-bot-roman',
                        language: 'python'
                    },
                    {
                        title: 'Kotlin Gradle Template',
                        description: 'Template for publishing Gradle libraries to JCenter.',
                        githubLink: 'https://github.com/LukasForst/maven-library',
                        language: 'kotlin'
                    },
                    {
                        title: '.NET Core Template',
                        description: 'Boilerplate for bigger projects using .NET Core 3.1.',
                        githubLink: 'https://github.com/LukasForst/dotnet-core-template',
                        language: 'csharp'
                    },
                    {
                        title: 'Bachelor Thesis',
                        description: 'Scheduling optimization jobs on distributed platform.',
                        githubLink: 'https://github.com/LukasForst/bachelor-thesis',
                        language: 'kotlin'
                    }
                ]
            }
        }
    }
</script>

<style scoped>
    #projects {
        text-align: center;
        /*display: inline-block;*/
        vertical-align: top;
        margin-top: 50px;

        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        max-width: 100%;
        overflow-x: hidden;
        justify-content: center;
    }
</style>