<template>
    <div id="app">
        <link rel="stylesheet"
              href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

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
        padding-top: 60px;
    }
    a {
        color: inherit;
    }
    #app {
        font-family: Avenir, Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
    }
</style>
