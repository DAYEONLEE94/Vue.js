<script>
  import SecondComponent from '@/components/SecondChild.vue';
  export default {
    data() {
      return {
        inputStr: "",
        inputEl: null,
      };
    },
    methods: {
      onclickHandler() {
        if(this.inputStr.trim() === "") {
          alert("입력값이 비어있습니다.")
          this.$refs.inputEl.focus();
          return;
        }
      }
    }
  };
</script>

<template>
  <form action="">
    <input type="text"  v-model="inputStr" ref="inputEl" />
    <button type="button" @click="onclickHandler">등록</button>
  </form>
  
</template>

<style></style>
