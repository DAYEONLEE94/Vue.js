<script>
  import SecondComponent from '@/components/SecondChild.vue';
import FirstChild from './components/FirstChild.vue';
  export default {
    data() {
      return {
        inputStr: "",
        inputEl: null,
        componentEl: null,
      };
    },
    methods: {
      onclickHandler() {
        console.log(this.$refs.componentEl.name)
      }
    }
  };
</script>

<template>
  <form action="">
    <input type="text"  v-model="inputStr" ref="inputEl" />
    <button type="button" @click="onclickHandler">등록</button>
  </form>
  
  <FirstChild ref="componentEl"/>
</template>

<style></style>
