<template>
  <div>
    <h1>Stuff to do</h1>
    <div v-bind:key="todo.id" v-for="todo in todos">
      <TodoItem v-bind:todo="todo"/>
    </div>
  </div>
</template>

<script>

import TodoItem from './TodoItem'

export default {
  name: 'Todos',
  components: { TodoItem },
  props: ['todos'],
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
