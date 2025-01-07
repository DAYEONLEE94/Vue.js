<script>
import TodoHeader from '@/components/TodoHeader.vue';
import TodoList from '@/components/TodoList.vue';
import TodoInput from '@/components/TodoInput.vue';
import { computed } from 'vue';
export default {
  data() {
    return {
      todo: [],
      current: "all", 
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

  updateTab(tab) {
    this.current = tab;
  },
  updateTodo(id) {
    this.todo = this.todo.map((v) => v.id === id ? {...v, completed: !v.completed} : v
  );
  },
  deleteTodo(id) {
    this.todo = this.todo.filter((v) => v.id !==id);
  },
 },

 computed: {
    computedTodo() {
      if(this.current === 'all') {
        return this.todo;
      }else if(this.current === 'completed') {
        return this.todo.filter((item) => item.completed);
      }
    }
  }
};

</script>

<template>
   <div class="todo">
    
      <TodoHeader :current @update-tab="updateTab" />
      <TodoList :computed-todo @delete-todo="deleteTodo" @update-todo="updateTodo" />
      <TodoInput @add-todo="addTodo" />     
    </div>
</template>

<style scoped></style>
