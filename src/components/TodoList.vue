<template>
<div>
  <TodoInputText v-model="newTodoText" v-on:keydown.enter="addTodo" v-on:click="addTodo"/>
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
    },
    methods: {
        addTodo(){
            const trimmedText = this.newTodoText.trim();
            if (trimmedText) {
                this.todos.push(trimmedText);
                this.newTodoText = "";
            }
        }
    }
};
</script>

<style>

</style>