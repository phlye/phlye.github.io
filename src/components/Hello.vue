<template>
  <div class="hello">
    <h1>Hello &#x1F44B;</h1>
    <p>My name is Charly.</p>
    <p>I'm a software engineer and musician based in London.</p>
    <p>Sometimes I try and make fun things:</p>
  </div>
</template>

<script>
export default {
  name: "Bio",
  props: {
    msg: String,
  },
};
</script>

<style scoped>
p {
  margin: 30px;
}
</style>
