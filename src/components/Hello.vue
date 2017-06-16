<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>{{ h2 }}</h2>
    <p v-for="todo in todos">{{todo}}</p>
    <p v="intro">{{intro}}</p>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data() {
    return {
      msg: 'what up, lauren?',
      h2: 'here is a h2',
      // todos: Array.from({ length: 40 }).map((e, i) => i),
      todos: ['hi', 'bye', 'see ya'],
      intro: 'this is the intro paragraph',
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
  color: #42b983;
}
</style>
