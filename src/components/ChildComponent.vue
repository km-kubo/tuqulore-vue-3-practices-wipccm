<template>
  <p>こんにちは、{{ user.name }}さん、{{ user.old }}才になりましたね。</p>
</template>

<script setup>
import { ref } from 'vue';

const props = defineProps({
  student: Object,
});

const user = ref(props.student);
</script>
