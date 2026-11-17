<!-- InfoCard: displays a title and a description -->
<template>
  <div class="info-card">
    <h3>{{ title }}</h3>
    <p>{{ description }}</p>
  </div>
</template>

<script setup>
defineProps({
  title: { type: String, required: true },
  description: { type: String, required: true }
})
</script>

<style scoped>
.info-card {
  background: white;
  border-left: 5px solid #1ea73c;
  border-radius: 8px;
  padding: 16px;
  box-shadow: 0 1px 4px rgba(0, 0, 0, 0.08);
}
h3 { margin: 0 0 8px; }
p { margin: 0; color: #4b5563; }
</style>
