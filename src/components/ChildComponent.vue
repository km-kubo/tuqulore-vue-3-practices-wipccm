<template>
  <p v-if="props.isShow">props "is-show"がtrueであれば見れます</p>
</template>

<script setup>
import { ref } from 'vue';

const props = defineProps({
  isShow: Boolean,
});

const show = ref(props.isShow);
</script>
