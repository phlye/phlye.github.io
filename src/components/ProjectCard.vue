<template>
  <a :href="url" target="_blank">
    <img :src="img" />
    <h2 :class="color">{{ name }}</h2>
    <p>
      {{ description }}
    </p>
    <p>
      {{ madeIn }}
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
    madeIn: String,
    color: String,
  },
};
</script>

<style scoped>
a {
  flex: 1;
  text-decoration: none;
  color: inherit;
  padding: 15px;
  margin: 10px;
  max-width: 465px;
  border-radius: 25px;
  border: 1px solid #2c3e5033;
  box-shadow: 1px 2px #2c3e5033;
  transition: all 0.25s ease-in-out 0.15s;
  transform: scale(1);
  transition: all 0.25s ease-in-out 0.15s;
}

a:hover {
  background-color: #dce5ee;
  box-shadow: 3px 4px #2c3e5033;
  transform: scale(1.01);
}

p {
  text-align: left;
  padding: 0px 25px;
}

img {
  width: 300px;
  height: 300px;
  object-fit: cover;
  border-radius: 25px;
}

h2 {
  text-align: right;
  padding: 0px 25px;
  letter-spacing: 3px;
}

h2.goldenrod {
  color: goldenrod;
}

h2.steelblue {
  color: steelblue;
}
</style>
