<script>
  export default{
    data() {
      return {
        message: '',
      };
    },
    methods: {
      AllText(event){
        this.message = event.target.value;
      }
    }
  }
</script>

<template>
 
    <input type="text" @input="AllText()">
    {{ message }}

</template>
<style></style>