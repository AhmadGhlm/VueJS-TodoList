<template>
  
</template>

<script>

import TodoInputText from '@/components/TodoInputText.vue';

export default {
    name: "app",
    components: {
        TodoInputText
    },
    data() {
        return {
            todos: ["Tomates", "Lait", "Gâteaux"]
        };
    }

};
</script>

<style>

</style>