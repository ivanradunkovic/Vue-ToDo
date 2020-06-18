<template>
  <div>
    <todo-list v-bind:todos="todos"></todo-list>
  </div>
</template>

<script>
import TodoList from './components/TodoList';

export default {
  name: 'app',
  components: {
  TodoList,
  },

data() {
    return {
      todos: [{
        title: 'Todo 1',
        project: 'Project 1',
        done: false,
      }, {
        title: 'Todo 2',
        project: 'Project 2',
        done: true,
      }, {
        title: 'Todo 3',
        project: 'Project 3',
        done: false,
      }, {
        title: 'Todo 4',
        project: 'Project 4',
        done: false,
      }],
    };
  },
};

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
