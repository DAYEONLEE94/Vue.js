<script>
export default {
  data() {
    return {
     message: '<h1>Hello, Vue JS!</h1>',
     name: '철수',
     age: 19,
    };
  },
};
</script>
<template>
 <h1 v-pre>{{ name }}</h1>
</template>
<style></style>
