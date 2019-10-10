<template>
  <div id="app" class="container">
    <h1 class="title is-1 has-text-white">My Todo List</h1>
    <TodoList />
  </div>
</template>

<script>
import TodoList from "@/components/TodoList.vue";

export default {
  name: "app",
  components: {
    TodoList
  }
};
</script>

<style lang="scss">
.container {
  margin: 100px 80px 0 100px;
  background-color: #131313;
  border-radius: 10px;
  color: #fff;
}

h1 {
  text-align: center;
}
</style>
