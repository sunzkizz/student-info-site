<!-- Students page: one StudentCard component repeated with v-for -->
<template>
  <section>
    <h1>Students</h1>

    <div class="grid">
      <StudentCard
        v-for="student in students"
        :key="student.id"
        :name="student.name"
        :course="student.course"
        :year="student.year"
        :email="student.email"
      />
    </div>

    <div class="actions">
      <AppButton label="Back to Home" color="orange" to="/" />
    </div>
  </section>
</template>

<script setup>
// Sample data (replace with your own classmates)
const students = [
  { id: 1, name: 'Aaron Hotchner', course: 'BSIT', year: 3, email: 'aaronhotch@example.com' },
  { id: 2, name: 'Penelope Garcia', course: 'BSIT', year: 2, email: 'blackqueen@example.com' },
  { id: 3, name: 'Spencer Reid', course: 'BSCS', year: 4, email: 'spence@example.com' },
  { id: 4, name: 'Emily Prentis', course: 'BSIS', year: 1, email: 'prentis.emily@example.com' }
]
</script>

<style scoped>
.actions { margin-top: 24px; }
</style>
