<!-- Root of the app: the layout (header + footer) wraps whichever page is active -->
<template>
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>

<style>
/* Global styles shared by every page */
* { box-sizing: border-box; }
body {
  margin: 0;
  font-family: system-ui, sans-serif;
  background: #f4f6fb;
  color: #1f2937;
}
.container { max-width: 960px; margin: 0 auto; padding: 24px 16px; }
.grid {
  display: grid;
  gap: 16px;
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
}
</style>
