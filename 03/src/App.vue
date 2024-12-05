<script>
  export default{
    data() {
      return {
        gender: 'male',
      };
    },
    methods: {
      printData(){
        console.log(this.gender);
      }
    }
    
  }
</script>

<template>
  <form id="loginForm">
    <label for="male">
      <input type="radio" id="male" v-model="gender" value="male"/>male
    </label>
    <label for="female">
      <input type="radio" id="female" v-model="gender" value="female"/>female
    </label>
    <button type="button" @click="printData">확인</button>

  </form>
</template>
<style></style>