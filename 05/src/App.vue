<script>
import CustomButton from '@/components/CustomButton.vue';
import DefaultLayout from '@/components/DefaultLayout.vue';

export default {
  components: {
    CustomButton,
    DefaultLayout,
  },
}
</script>
<template>
 <CustomButton>더블클릭</CustomButton>
 <DefaultLayout>
    <template v-slot:header>
      <header>
        <h1>Header</h1>
      </header>
    </template>
    <template #main>
      <main>
        <h1>Main</h1>
      </main>
    </template>
    <template #footer>
      <footer>
        <h1>Footer</h1>
      </footer>
    </template>
 </DefaultLayout>

</template>