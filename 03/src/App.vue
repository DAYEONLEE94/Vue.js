<script>
  export default{
    data(){
      return {
        number: 0,
      }
    },
    
    methods: {
      onclick1(number){
        if(this.number < 10){
          this.number++;
        }
      },
      onclick2(number){
        if(this.number > 0){
          this.number--;
        }
      },
    },
  }
</script>

<template>
  숫자 : {{ number }}
  <button @click="onclick1">증가</button>
  <button @click="onclick2">감소</button>
</template>

<style></style>