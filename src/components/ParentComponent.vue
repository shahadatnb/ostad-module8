<script setup>
import { ref } from 'vue';
import ChildComponent from './ChildComponent.vue';
const msg = ref('Hello World');
</script>

<template>
  <h1>Parent Component: {{ msg }}</h1>
  <ChildComponent v-model:message="msg"  />
</template>