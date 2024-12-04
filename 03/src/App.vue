<script>
export default {
  methods: {
    clickHandler(event){
      console.log(event);
    },  
  },
};
</script>

<template>
  <button v-on:click="clickHandler">클릭</button>
  <button @click="clickHandler">축약형 클릭</button>
</template>

<style></style>
