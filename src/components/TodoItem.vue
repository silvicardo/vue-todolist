<template>
  <div>
      <p>{{todo.title}}</p>
  </div>
</template>

<script>

export default {
  name: 'TodoItem',
  props: ['todo'],
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
