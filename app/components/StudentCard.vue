<!-- StudentCard: displays one student's information (data comes in through props) -->
<template>
  <div class="student-card">
    <div class="avatar">{{ initials }}</div>
    <h3>{{ name }}</h3>
    <p class="course">{{ course }}</p>
    <p>Year level: {{ year }}</p>
    <p>Email: {{ email }}</p>
  </div>
</template>

<script setup>
const props = defineProps({
  name: { type: String, required: true },
  course: { type: String, required: true },
  year: { type: Number, required: true },
  email: { type: String, default: 'N/A' }
})

// First letter of each word in the name, e.g. "Juan Dela Cruz" -> "JDC"
const initials = computed(() =>
  props.name.split(' ').map((word) => word[0]).join('')
)
</script>

<style scoped>
.student-card {
  background: white;
  border-radius: 12px;
  padding: 20px;
  text-align: center;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}
.avatar {
  width: 64px;
  height: 64px;
  margin: 0 auto 12px;
  border-radius: 50%;
  background: #1ea73c;
  color: white;
  font-size: 1.3rem;
  font-weight: 700;
  display: flex;
  align-items: center;
  justify-content: center;
}
h3 { margin: 0 0 4px; }
.course { color: #1ea73c; font-weight: 600; }
p { margin: 4px 0; font-size: 0.95rem; }
</style>
