<script>
  export default{

    methods: {
      submitHandler(event){
        event.preventDefault();
        console.log(this.uid, this.upw);
        },
      },
    };
</script>

<template>
  <form action="" @submit="submitHandler">
    아이디 <input type="text" id="uid" v-model="uid">
    패스워드 <input type="password" id="upw" v-model="upw">
  <button>로그인</button>
  </form>
  
</template>
<style></style>