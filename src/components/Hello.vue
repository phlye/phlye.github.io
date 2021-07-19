<template>
  <div class="hello">
    <h1>Hello &#x1F44B;</h1>
    <p>My name is Charly.</p>
    <p>I'm a software engineer and musician based in London.</p>
    <ul>
      <li>
        <a href="https://github.com/charlyflynn" target="_blank">- github</a>
      </li>
      <li>
        <a
          href="https://www.linkedin.com/in/charlie-flynn-86b278149"
          target="_blank"
          >- linkedin</a
        >
      </li>
      <li>
        <a class="disabled">- soundcloud</a>
      </li>
    </ul>
    <p>Sometimes I try and make fun things:</p>
  </div>
</template>

<script>
export default {
  name: "Hello",
  props: {
    msg: String,
  },
};
</script>

<style scoped>
p {
  margin: 30px;
}
ul {
  padding: 0;
  margin: 0;
  list-style-type: none;
}
li {
  display: inline;
}
a {
  text-decoration: none;
  margin: 15px;
}
a.disabled {
  cursor: not-allowed;
  text-decoration: line-through;
}
</style>
