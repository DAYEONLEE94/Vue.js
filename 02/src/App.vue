<script>
export default {
  data() {
    return {
     message: '<h1>Hello, Vue JS!</h1>',
     name: '철수',
     age: 19,
     className: 'red-color',
    };
  },
};
</script>
<template>
 <h1 v-bind:class="className">{{ name }}</h1>
</template>

<style>
.red-color{
  color: red;
}
</style>
