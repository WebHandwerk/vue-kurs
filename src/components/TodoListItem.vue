<template>
  <li :class="{finished:item.finished}">
    <input type="checkbox" :checked="item.finished">
    <button @click="toggleItem">toggle</button>
    {{item.name}}
  </li>
</template>

<script>
export default {
  name: "TodoListItem",
  props: ['item'],
  methods: {
    toggleItem() {
      this.$emit('toggle', this.item)
    }
  }
}
</script>

<style scoped>

</style>