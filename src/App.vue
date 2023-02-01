<template>
  <button @click="toggle = !toggle">toggle</button>
  {{ toggle }}
  <ChildComponent :is-show="toggle" />
</template>

<script setup>
import ChildComponent from './components/ChildComponent.vue';
import { ref } from 'vue';
const toggle = ref(false);
</script>

<style></style>
