<template>
  <button @click="toggle = !toggle">toggle</button>
  <ChildComponent :student="{ name: 'kubo', old: '30' }" />
</template>

<script setup>
import ChildComponent from './components/ChildComponent.vue';
import { ref } from 'vue';
const toggle = ref(false);
</script>

<style></style>
