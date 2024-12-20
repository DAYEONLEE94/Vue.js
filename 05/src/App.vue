<script>
import UserProfile from '@/components/UserProfile.vue';
export default {
  components: {
    UserProfile,
  },

data() {
  return {
    name: "김철수",
    age : 20,
  };
},
};
</script>
<template>
  <UserProfile name="김철수" age="20" /> 
  1번방법 - 숫자를 입력하고 싶어도 해당 코드로 작성하면 문자열로 들어간다.
  
  <UserProfile :name :age></UserProfile> 
  2번방법 - 숫자를 표현하고 싶으면 v-bind를 사용해 줘야한다.

  <UserProfile :name="`이다연`" :age="30"></UserProfile>
</template>