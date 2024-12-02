<script>
export default {
  methods: {
    clickHandler(){
      alert("click");
    },  
  },
};
</script>

<template>
  <button v-on:dblclick="clickHandler">더블 클릭</button>
  <button v-on:click="clickHandler">클릭</button>
  <button @click="clickHandler">축약형 클릭</button>
</template>

<style></style>
