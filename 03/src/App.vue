<script>
  export default {
    data(){
      return{
        color: 'blue',
        style: 'italic',
      };
    },
  }

</script>

<template>
  <h1 v-bind:style="{color: color, fontStyle: style}">Sample Text</h1>
</template>
<style></style>