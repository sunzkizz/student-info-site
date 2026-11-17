<!--
  AppButton: reusable button
  Props:
    label -> text shown on the button
    color -> blue | green | red | orange
    to    -> (optional) if given, the button becomes a link to that page
-->
<template>
  <component :is="to ? NuxtLink : 'button'" :to="to" :class="['btn', color]">
    {{ label }}
  </component>
</template>

<script setup>
import { NuxtLink } from '#components'

defineProps({
  label: { type: String, required: true },
  color: {
    type: String,
    default: 'blue',
    validator: (value) => ['blue', 'green', 'red', 'orange'].includes(value)
  },
  to: { type: String, default: '' }
})
</script>

<style scoped>
.btn {
  display: inline-block;
  padding: 10px 18px;
  border: none;
  border-radius: 8px;
  color: white;
  font-size: 1rem;
  cursor: pointer;
  text-decoration: none;
}
.btn:hover { opacity: 0.85; }
.blue   { background: #1ea73c; }
.green  { background: #2e5dc2; }
.red    { background: #dc2626; }
.orange { background: #ea580c; }
</style>
