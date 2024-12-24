<script>
import CustomButton from '@/components/CustomButton.vue';
import DefaultLayout from '@/components/DefaultLayout.vue';
import MixLayout from '@/components/MixLayout.vue';

export default {
  components: {
    CustomButton,
    DefaultLayout,
    MixLayout,
  },
}
</script>
<template>
 <CustomButton>더블클릭</CustomButton>
 <MixLayout>
    <template v-slot:header>
      <header>
        <h1>header</h1>
      </header>
    </template>
      <main>
        <h1>main</h1>
      </main>
    <template #footer>
      <footer>
        <h1>footer</h1>
      </footer>
    </template>
 </MixLayout>

</template>