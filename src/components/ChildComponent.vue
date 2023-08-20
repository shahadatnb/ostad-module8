<script setup>

const props  = defineProps(['message']);
const $emit = defineEmits(['update:message']);

const messageChenge = () => {
    $emit('update:message', 'Hello Vue');
}
    
</script>

<template>

  <h1>Child Compnent: {{ message }}</h1>

    <button @click="messageChenge()">Click</button>
</template>