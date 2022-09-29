<template>
  <p className="message">
    {{ message }}
  </p>
</template>

<script setup>
defineProps({
  message: {
    type: String,
    default: "Shizzle for nizzle",
  },
});
</script>

<style scoped></style>
