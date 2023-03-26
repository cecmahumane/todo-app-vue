<script>
import TodoList from './components/TodoList.vue'
import CreateTodo from './components/CreateTodo.vue'

export default {
  components: {
    TodoList,
    CreateTodo
  },  
  
  data() {
        return {
            todo: "This is a sample todo"
        }
    }
}
</script>

<template>
  <TodoList />
  <CreateTodo />
</template>

<style scoped>

</style>
