<script setup lang="ts">
import {ref} from 'vue';
import type {VDataTableHeader} from '@gits-id/table';

const states = ['active', 'inactive'];

const items = [...Array(30)].map((_, index) => ({
  index,
  name: `Nurul-${index}`,
  email: `Nurul-${index}@gmail.com`,
  age: index + 1 * 10,
  state: states[Math.floor(Math.random() * states.length)],
}));

const headers = ref<VDataTableHeader[]>([
  {
    value: 'index',
    text: 'ID',
  },
  {
    value: 'name',
    text: 'Name',
  },
  {
    value: 'email',
    text: 'Email',
  },
]);
</script>

<template>
  <!-- VDataTable is registered globally -->
  <VLogo />
  <VMultiSelect :items="items" />
  <VDataTable :items="items" :headers="headers" />
   <VRating :rating="2.5" :increment="0.5" />
</template>









