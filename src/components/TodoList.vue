<template>
  <ul>
    <TodoListItem
      v-for="todo in todos" :key="todo.id"
      :item="todo"
    />
  </ul>
</template>

<script>
import TodoListItem from "@/components/TodoListItem";
export default {
  name: "TodoList",
  data: () => ({
    todos: [
      {id: 1, finished: true, name: "Aufgabe 1"},
      {id: 2, finished: false, name: "Aufgabe 2"},
      {id: 3, finished: false, name: "Aufgabe 3"},
      {id: 4, finished: true, name: "Aufgabe 4"},
      {id: 5, finished: false, name: "Aufgabe 5"},
    ]
  }),
  components: {
    TodoListItem
  }
}
</script>

<style scoped>

</style>