<template>
  <li :class="{finished:item.finished}">
    <input type="checkbox" :checked="item.finished">
    <a href="">zeigen</a>
    {{item.name}}
  </li>
</template>

<script>
export default {
  name: "TodoListItem",
  props: ['item']
}
</script>

<style scoped>

</style>