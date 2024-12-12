<script>
  import SecondComponent from '@/components/SecondChild.vue';
  export default {

    data() {
      return {
        number: 0,
      };
    },
    beforeCreate() {
      console.log('beforeCreate');
    },
    created() {
      console.log('created');
    },
    beforeMount() {
      console.log('boforeMount');
    },
    mounted() {
      console.log('mounted');
    },
    beforeUpdate() {
      console.log('beforeUpdate');
    },
    updated() {
      console.log('update');
    },
    beforeUnmount() {
      console.log('beforeUnmount');
    },
    unmounted() {
      console.log('unmounted');
    },  

    methods: {
      increment() {
        this.number++;
      }
    }
  };
</script>

<template>
  <h1>count : {{ number }}</h1>
  <FirstChild v-if="number % 2 === 0" />
  <button @click="increment">증가</button>
  
</template>

<style></style>
