<script>
  export default {
    data() {
      return {
        inputMsg: "",
      };
    },
    emits: ["add-todo"],

    methods: {
      addTodo() {
        this.$emit("add-todo", this.inputMsg);
        this.inputMsg = "";
      },
    },
}
</script>

<template>
     <div class="todo__input">
        <input
          v-model="inputMsg"
          type="text"
          class="todo__input-text"
          placeholder="할 일을 입력하세요." 
          @keyup.enter="addTodo"
        />
        <button class="todo__input-btn" @click="addTodo">등록</button>
      </div>
</template>