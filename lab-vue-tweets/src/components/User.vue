<script setup>
defineProps({
  user: {
    type: Object,
    define: () => ({
      name: "Michael Jordan",
      handle: "@jumpjOR",
    }),
  },
});
</script>

<template>
  <span className="user">
    <span className="name">{{ user.name }}</span>
    <span className="handle">{{ user.handle }}</span>
  </span>
</template>

<style scoped></style>
