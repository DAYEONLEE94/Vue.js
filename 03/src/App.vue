<script>
export default {
  data(){
    return {
      number: 0
    };
  },
  methods: {
    onClick(){
      this.number++;
    },    
  },
};
</script>

<template>
  <h1 v-once>{{ number }}</h1>c
  <button @click="onClick">증가</button>
</template>

<style></style>
