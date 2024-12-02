<script>
export default {
  data() {
    return {
    fruits: ['apple', 'banana', 'orange'],
    };
  },
};
</script>
<template>
  <h1>fruits 데이터 반복 결과</h1>
  <ul>
    <li v-for="(value, index) in fruits" :key="index">
       인덱스: {{ index }}, 값: {{ value }}
    </li>
  </ul>
</template>

<style>
</style>
