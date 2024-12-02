<script>
export default {
  data() {
    return {
     visible: true,
     unvisible: false,
     condition: 'F',
    };
  },
};
</script>
<template>
 <h1 v-if="visible">이 요소는 렌더링 됩니다.</h1>
 <h1 v-if="unvisible">이 요소는 렌더링되지 않습니다.</h1>

 <h1 v-if="condition === 'A'">condition {{ condition }} 입니다.</h1>
 <h1 v-else-if="condition === 'B'">condition {{ condition }} 입니다.</h1>
 <h1 v-else-if="condition === 'C'">condition {{ condition }} 입니다.</h1>
 <h1 v-else-if="condition === 'D'">condition {{ condition }} 입니다.</h1>
 <h1 v-else="condition">condition이 없습니다.</h1>

</template>

<style>
</style>
