<script>
import { computed } from 'vue';

  export default {
    props: {
      computedTodo: {
        type: Array,
        default() {
          return [];
        },
      },
    },
    emits: ["delete-todo", "update-todo"],
  };
</script>

<template>
    <div class="todo__list">
        <div v-for="item in computedTodo" :key="item.id" class="todo__item" :class="{'todo__item--completed': item.completed}">
          <input type="checkbox" :id="`chk${item.id.toString()}`" :checked="item.completed" @click="$emit('update-todo', item.id)" />
          <label :for="`chk${item.id.toString()}`" class="todo__checkbox-label"></label>
          <span class="todo__item-text">{{item.msg}}</span>
          <span class="material-symbols-outlined todo__delete-icon" @click="$emit('delete-todo', item.id)">delete</span>



        </div>
        <!-- 할 일 목록이 없을 때 -->
        <div v-if="computedTodo.length === 0" class="todo__item--no" style="display: none">
          <p>할일 목록이 없습니다.</p>
        </div>
      </div>
</template>
