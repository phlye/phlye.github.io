<template>
  <Hello />
  <Projects />
  <Disclaimer />
</template>

<script>
import Hello from "./components/Hello.vue";
import Projects from "./components/Projects.vue";
import Disclaimer from "./components/Disclaimer.vue";

export default {
  name: "App",
  components: {
    Projects,
    Hello,
    Disclaimer,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css?family=Roboto+Mono");

html,
body {
  font-family: "Roboto Mono", sans-serif;
}

#app {
  font-family: "Roboto Mono", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.projectContainer {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}
</style>
