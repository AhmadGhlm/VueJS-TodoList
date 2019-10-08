<template>
<div>
  <TodoInputText v-model="newTodoText" />
  <TodoListItem :todos="todos" />
</div>
</template>

<script>

import TodoInputText from '@/components/TodoInputText.vue';
import TodoListItem from '@/components/TodoListItem.vue';

export default {
    name: "app",
    components: {
        TodoInputText,
        TodoListItem
    },
    data() {
        return {
            newTodoText: "",
            todos: ["Tomates", "Lait", "Gâteaux"]
        };
    }

};
</script>

<style>

</style>