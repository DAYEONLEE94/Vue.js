<script>
  export default {
    emits: ['print-hello'],

    methods: {
        parentEventCall() {
            this.$emit('onPrint-hello');
        }
    }
}

</script>
<template>
    <button @click="parentEventCall">클릭</button>
</template>