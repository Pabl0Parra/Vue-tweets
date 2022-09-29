<template>
  <div className="tweet">
    <ProfileImage :image="image" :ImageAlt="ImageAlt" />
    <div className="body">
      <div className="top">
        <User :user="user" />
        <TimeStamp v-bind:timestamp="timestamp" />
      </div>
      <Message v-bind:message="message" />
      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script setup>
import ProfileImage from "./ProfileImage.vue";
import Actions from "./Actions.vue";
import Message from "./Message.vue";
import User from "./User.vue";
import TimeStamp from "./TimeStamp.vue";

defineProps({
  message: {
    type: String,
  },
  timestamp: {
    type: String,
  },
  user: {
    type: Object,
  },
  image: {
    type: String,
  },
  ImageAlt: {
    type: String,
  },
});
</script>

<style scoped>
a {
  color: #42b983;
}

/* .profile {
  width: 30px;
  height: 30px;
} */
</style>
