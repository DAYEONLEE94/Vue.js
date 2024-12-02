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
  콧수염 문법 : <h1>{{ message }}</h1>
  v-html디렉티브 : <div v-html="message"></div>
  v-text 디렉티브 : <h1 v-text="message"></h1>
</template>
<style></style>
