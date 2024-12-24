<script>
import FirstChild from '@/components/FirstChild.vue';

export default {
  components: {
    FirstChild,
  },
  
  mounted() {
    console.log(this.$refs.childRef.childNum);
    console.log(this.$refs.childRef.childNumOddAdd);
    console.log(this.$refs.childRef.getChildNum());
  }
};
</script>
<template>
 <h1>App</h1>
 <FirstChild ref="childRef"/>

</template>