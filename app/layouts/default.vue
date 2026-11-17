<!-- The SAME header and footer are used on every page through this layout -->
<template>
  <div class="layout">
    <AppHeader />
    <main class="container">
      <slot />
    </main>
    <AppFooter />
  </div>
</template>

<style scoped>
.layout { min-height: 100vh; display: flex; flex-direction: column; }
main { flex: 1; width: 100%; }
</style>
