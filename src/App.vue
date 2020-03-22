<template>
    <div id="app">
        <About/>
        <Projects/>
    </div>
</template>

<script>

    import About from "./componenets/About";
    import Projects from "./componenets/Projects";

    export default {
        name: 'App',
        components: {
            Projects,
            About
        }
    }
</script>

<style>
    body {
        overflow: hidden;
        height: 100vh;
    }

    a {
        color: inherit;
        text-decoration: none;
    }

    #app {
        font-family: Avenir, Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }
</style>
