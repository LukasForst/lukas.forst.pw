<template>
  <div id="app">
    <link rel="stylesheet"
          href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

    <Headline/>
    <About/>
    <Projects/>
  </div>
</template>

<script>

import Headline from './componenets/Headline';
import Projects from './componenets/Projects';
import About from '@/componenets/About';

export default {
  name: 'App',
  components: {
    About,
    Projects,
    Headline
  }
};
</script>

<style>
body {
  padding-top: 40px;
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
