<template>
  <div id="app">
    <!-- Todo components get App component data->todos as a prop -->
    <Todos v-bind:todos="todos" />
  </div>
</template>

<script>

//import child components
import Todos from './components/Todos'

//export actual component
export default {
  name: 'app',
  components: {
    Todos
  },
  data() {
    return {//
      todos: [
        { id: 1, title: 'uscire', completed: false },
        { id: 2, title: 'studiare', completed: false },
        { id: 3, title: 'dormire', completed: false },
        { id: 4, title: 'React', completed: false },
      ]
    }
  }
}
</script>

<!-- Global Styles -->
<style>

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}

</style>
