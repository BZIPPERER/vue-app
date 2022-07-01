<template>
  <div class="hello">
    <h1>{{ msg }}</h1><a href="www.bild.de" >Gas Notstand</a>
      For a guide and reipes on how to configure / customize this project -<br/>
      check out the pizza
    <h3>Katze im Sack [Sackplatzer]</h3>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: green;
}
</style>
