<script>
  export default{
    data() {
      return {
        firstName: 'Gildong',
        lastName: 'Hong',
      };
    },

    computed: {
      fullName() {
        console.log('fullName');
        return `${this.lastName} ${this.firstName}`;
        // return this.firstName + this.lastName;
      }, 
    },
    };
</script>

<template>
 <h1>{{ fullName }}</h1> 
</template>
<style></style>