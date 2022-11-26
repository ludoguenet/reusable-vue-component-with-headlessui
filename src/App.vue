<template>
  <div class="mx-auto container">
    <select-options
        :options="people"

        v-model="userId"
      />
  </div>
</template>

<script setup lang="ts">
import SelectOptions from "./components/SelectOptions.vue";
import {ref} from 'vue';

const userId = ref<number>(1);

const people = [
  { id: 1, name: 'Wade Cooper' },
  { id: 2, name: 'Arlene Mccoy' },
  { id: 3, name: 'Devon Webb' },
  { id: 4, name: 'Tom Cook' },
  { id: 5, name: 'Tanya Fox' },
  { id: 6, name: 'Hellen Schmidt' },
]
</script>
