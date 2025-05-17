<template>
  <p class="message">{{content}} </p>
</template>

<script setup>
const props = defineProps({
  content: {
    type: String,
    required: true,
  },
});
</script>

<style></style>
