<template>
  <img v-bind:src="image" className="profile" :ImageAlt="profile" />
</template>

<script setup>
defineProps({
  image: {
    type: String,
    default: "https://i.imgur.com/b0EdHVV.jpg",
  },
  ImageAlt: {
    type: String,
    default: "Some random text",
  },
});
</script>

<style scoped></style>
