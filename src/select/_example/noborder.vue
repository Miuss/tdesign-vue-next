<template>
  <t-select
    v-model="value"
    :bordered="false"
    style="width: 200px"
    placeholder="-请选择-"
    clearable
    auto-width
    :options="options"
  />
</template>
<script setup>
import { ref } from 'vue';

const options = [
  {
    label: '已选择的选项',
    value: '1',
  },
  {
    label: '短的选项二',
    value: '2',
  },
  {
    label: '很长很长很长的选项三',
    value: '3',
  },
];

const value = ref('1');
</script>
