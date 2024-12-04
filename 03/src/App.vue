<script>
export default {
  methods: {
    onKeyuphandler(event){
      alert("eneter!");
    },  
  },
};
</script>

<template>
  <input @keyup.enter="onKeyuphandler"></input>
</template>

<style></style>
