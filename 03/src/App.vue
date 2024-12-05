<script>
  export default{ 
    data() {
      return {
        fruits: ['banana', 'orange'],
      };
    },

    methods: {
      printData() {
        console.log(this.fruits);
      },
    },
  }


</script>

<template>
  <form id="loginForm">
    <label for="banana">
      <input type="checkbox" id="banana" v-model="fruits" value="banana"/>banana
    </label>
    <label for="orange">
      <input type="checkbox" id="orange" v-model="fruits" value="orange"/>orange
    </label>
    <label for="apple">
      <input type="checkbox" id="orange" v-model="fruits" value="apple"/>apple
    </label>
    <button type="button" @click="printData">확인</button>
  </form>
 
</template>

<style></style>
