<script>
  export default {
    props: {
      current: {
        type: String,
        default() {
          return "all";
        },
      },
    },
    emits: ["update-tab"],
  };
</script>
<template>
    <div class="todo__title">
        <h1 class="todo__text">Todo List</h1>
        <ul class="todo__tab">
          <li :class="{'todo__tab--active': current === 'all'}" @click="$emit('update-tab',  'all')">전체</li>
          <li :class="{'todo__tab--active': current === 'completed'}" @click="$emit('update-tab',  'completed')">완료</li> 
        </ul>
      </div>
</template>