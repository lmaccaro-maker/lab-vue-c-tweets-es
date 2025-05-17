<template>
  <span class="timestamp">{{ time }}</span>
</template>

<script setup>
const props = defineProps({
  time: {
    type: String,
    required: true,
  },
});
</script>

<style scoped></style>
