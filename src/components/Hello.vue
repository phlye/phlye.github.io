<template>
  <div class="hello">
    <p>Hello &#x1F44B; My name is Charly.</p>
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
  margin: 50px;
}
</style>
