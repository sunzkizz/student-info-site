<!-- AppFooter: website footer -->
<template>
  <footer class="footer">
    <p>© {{ year }} Student Information Website · Built with reusable components. This is a dummy that is used for student project.</p>
  </footer>
</template>

<script setup>
const year = new Date().getFullYear()
</script>

<style scoped>
.footer { background: #111827; color: #9ca3af; text-align: center; padding: 16px; }
.footer p { margin: 0; font-size: 0.9rem; }
</style>
