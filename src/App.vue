<template>
  <div id="app">
    Hi, {{name_first}}

    <TodoList />

    <button @click="test">Test</button>

  </div>
</template>

<script>
import TodoList from "@/components/TodoList";

export default {
  name: 'App',
  data: () => ({
    name_first: 'Reinhard',
  }),
  methods: {
    test() {
      alert("hi")
    }
  },
  components: {
    TodoList
  }

}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
  margin-top: 60px;
}

li {
  list-style: none;
}

.finished {
  text-decoration: line-through;
}
</style>
