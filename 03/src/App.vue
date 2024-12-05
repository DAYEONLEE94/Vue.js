<script>
export default {
  data(){
    return {
      number1: 0,
      number2: 0,
    };
  },
  methods: {
    onClick1(){
      this.number1++;
    },
    onClick2(){
      this.number2++;
    },    
  },
};
</script>

<template>
  <h1 v-memo="[number1, number2]">{{ number1 }} / {{number2}}</h1>
  <button @click="onClick1">증가</button>
  <button @click="onClick2">증가</button>
</template>

<style></style>
