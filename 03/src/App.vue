<script>
  export default{
    data(){
      return{
        message: '',
      };
    },
    methods: {
      printData() {
        console.log(this.message);      
      }
      
    },
  }


</script>

<template>
  <form id="loginCheck">
   <textarea v-model="message"></textarea>
    <button type="button" @click="printData">데이터출력</button>
  </form>
 
</template>

<style></style>
