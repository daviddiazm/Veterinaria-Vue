<script setup lang='js'>
  import AppHeader from './components/AppHeader.vue'
  import AppForm from './components/AppForm.vue';
import { ref } from 'vue';

  const pacientes = ref([])
</script>

<template >
  <!-- <div class="container mx-auto mt-2"> -->
  <div class="container mx-auto pt-2 lg:px-20">
    <AppHeader/>

    <div class="flex flex-col mt-12 md:flex-row">
      <AppForm/>

      <div class=" mt-5 md:w-1/2 ">
        <h2 class="text-3xl text-center font-bold">Lista de Pacientes</h2>
        <p
          v-if="pacientes.length <= 0"
          class="text-xl text-center mt-12">
          No hay pacientes
        </p>
      </div>
    </div>

  </div>
</template>

<style>
</style>
