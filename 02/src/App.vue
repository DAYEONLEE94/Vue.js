<script>
export default {
  data() {
    return {
      name: 'abc',
      age: 19,
    };
  },
};
</script>
<template>
 <p>저의 이름은 {{ name }} 입니다.</p>
 <p>저의 나이는 {{ age }} 입니다.</p>
 {{ 10 * 20 * 30 }}
 {{ name.toUpperCase() }}
</template>
<style></style>
