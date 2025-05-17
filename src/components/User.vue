<template>
  <div class="user-info">
    <span class="name">{{ userData.name }}</span>
  <span class="handle">{{ userData.handle }}</span>
    
  </div>
</template>

<script setup>
const props = defineProps({
  userData: {
    type: Object,
    required: true,
  },
});
</script>


<style scoped></style>





