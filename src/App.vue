<template>
  <div id="app">
    <div class="container">
      <h1 id="todo-header">Todos</h1>
      <AddTodo />
      <FilterTodos />
      <Todos />
    </div>
  </div>
</template>

<script>
import FilterTodos from "./components/FilterTodos.vue";
import AddTodo from "./components/AddTodo.vue";
import Todos from "./components/Todos.vue";

export default {
  name: "App",
  components: {
    Todos,
    AddTodo,
    FilterTodos
  }
};
</script>

<style>
@import "../node_modules/@fortawesome/fontawesome-free/css/all.css";

body {
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
  line-height: 1.6;
  background: #e8f7f0;
}
.container {
  max-width: 1100px;
  margin: auto;
  overflow: auto;
  padding: 0 2rem;
}
#todo-header {
  text-align: center;
}
</style>
