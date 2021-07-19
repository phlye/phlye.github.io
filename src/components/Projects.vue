<template>
  <div class="projectsContainer">
    <ProjectCard
      name="acordes"
      :img="require('@/assets/acordes.png')"
      url="http://acordes.netlify.app"
      description="a real-time browser based chord recognition and naming tool, for MIDI keyboards."
      madeIn=" built using react and the chrome web MIDI API."
      color="goldenrod"
    />
    <ProjectCard
      name="deimos project"
      :img="require('@/assets/deimos.png')"
      url="http://deimos-project.netlify.app"
      description="an attempt to visualise the scale of inequality in the UK."
      madeIn=" built using three.js and react-three-fiber (WIP)."
      color="steelblue"
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
  border-top: 1px solid #2c3e5033;
  border-bottom: 1px solid #2c3e5033;
  padding: 25px 0px;
}
</style>
