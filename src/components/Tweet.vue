<script setup>
import Actions from "./Actions.vue";
import Message from "./Message.vue";
import ProfileImage from "./ProfileImage.vue";
import Timestamp from "./Timestamp.vue";
import User from "./User.vue";

const props = defineProps({
  tweet: {
    type: Object,
    required: true,
  },
});
</script>

<template>
  <div class="tweet">
    <ProfileImage :image="tweet.user.image" />

    <div class="body">
      <Timestamp :time="tweet.timestamp" />

      <div class="top">
        <User :userData="tweet.user" />
      </div>

      <Message :content="tweet.message" />

      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>
