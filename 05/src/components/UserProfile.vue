<script>
    export default {
        props: ["name", "age"],
        created() {
            console.log(typeof this.age);
        },
    };
    
</script>
<template>
    <h1>UserProfile</h1>
    <p>{{ name }} / {{ age }}</p>
    
</template>