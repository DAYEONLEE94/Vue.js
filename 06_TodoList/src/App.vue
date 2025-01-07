<script>
import TodoHeader from '@/components/TodoHeader.vue';
import TodoList from '@/components/TodoList.vue';
import TodoInput from '@/components/TodoInput.vue';
export default {
  data() {
    return {
      todo: [],
    };
  },
  components: {
    TodoHeader,
    TodoList,
    TodoInput,
  },
  methods: {
    addTodo(inputMsg) {
    const item = {
      id: Math.random(),
      msg: inputMsg,
      completed: false,
    };
    this.todo.push(item);
  },
  }
};

</script>

<template>
   <div class="todo">
    {{ JSON.stringify(todo, null, 2) }}
      <TodoHeader />
      <TodoList />
      <TodoInput @add-todo="addTodo" />     
    </div>
</template>

<style scoped></style>
