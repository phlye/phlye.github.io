<template>
  <div class="hello">
    <h1>hello &#x1F44B;</h1>
    <p>my name is Charly.</p>
    <p>i'm a software engineer and musician based in London.</p>
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
    <p>sometimes I try and make fun things:</p>
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
  display: inline-block;
}
a {
  text-decoration: none;
  margin: 15px;
  padding: 8px;
  outline: none;
  font-weight: bold;
  color: inherit;
  border: 1px solid goldenrod;
  border-radius: 5px;
}

a.disabled {
  cursor: not-allowed;
  text-decoration: line-through;
}
</style>
