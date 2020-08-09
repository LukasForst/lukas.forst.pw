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
                projects: [
                    {
                        title: 'Katlib',
                        description: 'Collection of extension functions for Kotlin.',
                        githubLink: 'https://github.com/LukasForst/katlib',
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
                        title: 'Charon-Slack DevOps',
                        description: 'DevOps porn for Slack Bots onboarding.',
                        githubLink: 'https://github.com/LukasForst/slack-onboarding-bot',
                        language: 'python'
                    },
                    {
                        title: 'Ganymede',
                        description: 'Wire\'s digital signatures backend.',
                        githubLink: 'https://github.com/wireapp/ganymede',
                        language: 'kotlin'
                    },
                    {
                        title: 'Wire Backup Export',
                        description: 'Tool for reading Wire Client backups.',
                        githubLink: 'https://github.com/LukasForst/wire-backup-export',
                        language: 'kotlin'
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
                        title: 'Printing Company',
                        description: 'Application for company management.',
                        githubLink: 'https://github.com/LukasForst/printing-company',
                        language: 'react'
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
                    },
                    {
                        title: 'Students Phishing',
                        description: 'Blog post on how we hacked students on CTU.',
                        githubLink: 'https://github.com/LukasForst/BSY',
                        language: 'python'
                    },
                    {
                        title: 'Thinkfan Helper',
                        description: 'Tool fixing Thinkfan settings on some kernels.',
                        githubLink: 'https://github.com/LukasForst/thinkfan-helper',
                        language: 'python'
                    },
                    {
                        title: 'DataVID-19',
                        description: 'Hackaton tool for medical speech2text.',
                        githubLink: 'https://github.com/tomaskourim/datavid/',
                        language: 'python'
                    },
                    {
                        title: 'Speech2Text',
                        description: 'Speech to text with NodeJS and websockets.',
                        githubLink: 'https://github.com/LukasForst/datavid-speech2text',
                        language: 'nodejs'
                    },
                    {
                        title: 'Curriculum Vitae',
                        description: 'My not necessarily up to date CV.',
                        githubLink: 'https://github.com/LukasForst/cv',
                        language: 'tex'
                    }
                ]
            }
        }
    }
</script>

<style scoped>
    .projects-container {
        margin-top: 50px;
        margin-left: 5%;
        margin-right: 5%;
    }

    #projects {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: space-evenly;
    }
</style>
