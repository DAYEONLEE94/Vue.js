<script>
  import SecondComponent from '@/components/SecondChild.vue';
  export default {
    beforeCreate() {
      console.log('firstChild beforeCreate');
    },
    created() {
      console.log('firstChild created');
    },
    beforeMount() {
      console.log('firstChild boforeMount');
    },
    mounted() {
      console.log('firstChild mounted');
    },
    beforeUnmount() {
      console.log('firstChild beforeUnmount');
    },
    unmounted() {
      console.log('firstChild unmounted');
    },  
  };
</script>

<template>
 <h1>FirstChildComponent</h1>

</template>

<style></style>
