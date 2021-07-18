<template>
  <a :href="url" target="_blank">
    <img :src="img" />
    <h2>{{ name }}</h2>
    <p>
      {{ description }}
    </p>
  </a>
</template>

<script>
export default {
  name: "ProjectCard",
  props: {
    name: String,
    url: String,
    img: String,
    description: String,
  },
};
</script>

<style scoped>
a {
  display: block;
  text-decoration: none;
  color: inherit;
  width: 450px;
  height: 450px;
  padding: 15px;
  margin: 15px;
  border-radius: 25px;
  border: 1px solid #2c3e5033;
  box-shadow: 1px 2px #2c3e5033;
  transition: all 0.25s ease-in-out 0.15s;
  transform: scale(1);
  transition: all 0.25s ease-in-out 0.15s;
}

a:hover {
  background-color: #f9f9f9;
  box-shadow: 3px 4px #2c3e5033;
  transform: scale(1.01);
}

img {
  width: 300px;
  height: 300px;
  object-fit: cover;
  border-radius: 25px;
}

h2 {
  color: goldenrod;
}
</style>
