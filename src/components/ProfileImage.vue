<template>
  <img :src="image" class="profile" alt="profile" />
  <div></div>
</template>

<script setup>
const props = defineProps({
  image: {
    type: String,
    required: true,
  },
});
</script>

<style scoped>
img {
  width: 48px;
  height: 48px;
  border-radius: 50%;
}
</style>
