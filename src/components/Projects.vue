<template>
  <div class="projectsContainer">
    <ProjectCard
      img="../assets/acordes.png"
      name="acordes"
      url="http://acordes.netlify.app"
      description="a browser based chord analysis/naming tool that works with both MIDI
      keyboards as well as point and click"
    />
    <ProjectCard
      img="../assets/acordes.png"
      name="phobos project"
      url="http://animated-garbanzo.netlify.app"
      description="an attempt to show the scale of inequality built using three.js/react-three-fiber (WIP)"
    />
  </div>
</template>

<script>
import ProjectCard from "./ProjectCard.vue";

export default {
  name: "App",
  components: {
    ProjectCard,
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Roboto+Mono");

html,
body {
  font-family: "Roboto Mono", sans-serif;
}

.projectsContainer {
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}
</style>
