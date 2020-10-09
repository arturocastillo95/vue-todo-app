<template>
  <div id="app">
    <Todos v-bind:todos="todos"/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
  import Todos from './components/Todos'

  export default {
    name: 'App',
    components: {
      Todos
    },
    data() {
      return {
        todos: [
          {
            id: 1,
            title: 'Home work',
            completed: false,
          },
          {
            id: 2,
            title: 'Work',
            completed: false,
          },
          {
            id: 3,
            title: 'Work-HARD',
            completed: false,
          },
        ],
      }
    }
  }
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 1rem;
}
</style>
